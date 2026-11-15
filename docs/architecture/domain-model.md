# Perch — Conceptual Domain Model

**Note:** This is a platform-neutral conceptual model. The move to web-first changes navigation and interaction design, not the core reader, book and post concepts. This is not a final database schema.

## 1. Phase 1 Entities

```mermaid
erDiagram
    USER ||--o| READER_PROFILE : has
    USER ||--o{ POST : creates
    USER ||--o{ SHELF_ENTRY : maintains
    USER ||--o{ FOLLOW : follows
    USER ||--o{ REACTION : makes
    USER ||--o{ COMMENT : writes
    USER ||--o{ NOTIFICATION : receives

    BOOK ||--o{ POST : referenced_by
    BOOK ||--o{ SHELF_ENTRY : appears_in
    BOOK ||--o{ BOOK_GENRE : classified_as
    GENRE ||--o{ BOOK_GENRE : contains
    BOOK ||--o{ BOOK_AUTHOR : credits
    AUTHOR ||--o{ BOOK_AUTHOR : credited_on

    POST ||--o| REVIEW_DETAILS : may_have
    POST ||--o{ REACTION : receives
    POST ||--o{ COMMENT : receives

    USER ||--o{ CONTENT_REPORT : submits
    POST ||--o{ CONTENT_REPORT : reported_in
    BOOK ||--o{ PURCHASE_LINK : links_to

    USER {
        string id
        string email
        string account_status
        datetime created_at
    }

    READER_PROFILE {
        string user_id
        string display_name
        string bio
        string avatar_url
        string privacy_setting
    }

    BOOK {
        string id
        string title
        string description
        string cover_image_url
        string isbn
        string publication_date
    }

    AUTHOR {
        string id
        string name
    }

    BOOK_AUTHOR {
        string book_id
        string author_id
        string role
    }

    GENRE {
        string id
        string name
    }

    BOOK_GENRE {
        string book_id
        string genre_id
    }

    POST {
        string id
        string user_id
        string book_id
        string post_type
        string body
        boolean contains_spoilers
        datetime created_at
    }

    REVIEW_DETAILS {
        string post_id
        number enjoyment_rating
        number expectation_match_rating
    }

    SHELF_ENTRY {
        string id
        string user_id
        string book_id
        string shelf_status
        datetime updated_at
    }

    FOLLOW {
        string follower_user_id
        string followed_user_id
        datetime created_at
    }

    REACTION {
        string id
        string user_id
        string post_id
        string reaction_type
    }

    COMMENT {
        string id
        string user_id
        string post_id
        string body
        datetime created_at
    }

    PURCHASE_LINK {
        string id
        string book_id
        string retailer_name
        string destination_url
    }

    NOTIFICATION {
        string id
        string user_id
        string notification_type
        string related_entity_id
        datetime created_at
        datetime read_at
    }

    CONTENT_REPORT {
        string id
        string reporter_user_id
        string post_id
        string reason
        datetime created_at
    }
```

## 2. Domain Rules

1. A reader has one shelf status per book in the simplest MVP model.
2. Enjoyment and expectation-match ratings are separate values.
3. Expectation match measures whether a book met the reader's expectations, not whether the reader personally enjoyed it.
4. A post may be a reaction, recommendation or structured review. Validate whether separate post types are necessary.
5. A post references one book in the initial release. Multi-book posts can be considered later.
6. Purchase links lead to external retailers. Perch does not own checkout or fulfilment in Phase 1.
7. Taste similarity can be derived from reader activity and preferences; it may not need a persisted entity initially.
8. Similarity indicators should avoid implying certainty and should expose evidence where practical.
9. Profile and shelf visibility rules must be defined before implementation.
10. Reporting and moderation should be supported, even if moderation operations are initially lightweight.

## 3. Future-Phase Extensions

These are not Phase 1 requirements.

### Writer ecosystem
- `WRITING_WORK`
- `CHAPTER`
- `WRITING_FEEDBACK`
- `WRITER_FOLLOW`

### Institution ecosystem
- `INSTITUTION`
- `PROGRAM`
- `COHORT`
- `EVALUATION_RUBRIC`
- `EVALUATION`

### Publisher ecosystem
- `PUBLISHER`
- `PUBLISHER_CATALOG_ENTRY`
- `SPONSORED_CAMPAIGN`
- `CAMPAIGN_METRIC`

## 4. Open Domain Decisions

- Is a book represented as a work, an edition, or both?
- Can one post reference multiple books?
- Are ratings numeric, categorical or both?
- Can readers create custom shelves?
- Which profile and shelf fields are public by default?
- How should duplicate book metadata and merged editions be handled?
- What minimum sample size is needed before displaying aggregate expectation-match or taste-match signals?
