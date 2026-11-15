# Perch — User Journey Maps

**Status:** Draft for validation  
**Scope:** Phase 1 reader MVP  
**Audience:** Product, UX, engineering, research

## Purpose

These journeys describe the reader experience Perch is intended to support. They are product hypotheses, not validated findings. Use research and prototype testing to confirm or revise them.

## Journey 1 — New reader onboarding and first discovery

**User goal:** Find books that fit their interests without having to build a network first.

| Stage | User action | User question / thought | Potential friction | Product opportunity |
|---|---|---|---|---|
| Entry | Opens Perch and creates an account | “What is this, and is it useful to me?” | Value proposition unclear | Explain reader-led discovery in onboarding |
| Preferences | Selects favourite genres and a few books/authors they like | “Will this help personalize what I see?” | Too many onboarding questions | Ask only for high-value optional signals |
| First feed | Views a starter discovery feed | “Are these books relevant?” | Empty or generic feed | Use selected genres and curated starter content |
| Book exploration | Opens a book page | “What do readers actually think?” | Book page lacks useful context | Show reviews, reader profiles and rating counts |
| Decision | Saves book to Want to Read or opens a retailer link | “Should I remember this or buy it?” | Purchase link unclear or unavailable | Make save and external purchase actions distinct |
| Return | Comes back to browse | “Is there anything new for me?” | Repetitive feed | Refresh discovery based on explicit interactions |

**Success signals:** onboarding completion, first book detail view, first shelf addition, return visit.

## Journey 2 — Evaluate a book before buying

**User goal:** Decide whether a promoted or recommended book is likely to meet expectations.

| Stage | User action | User question / thought | Potential friction | Product opportunity |
|---|---|---|---|---|
| Trigger | Sees a book on social media, hears about it from a friend, or encounters it in Perch | “Is this book worth my time and money?” | Promotion may overstate the experience | Make it easy to search the catalog |
| Search | Searches for the title or author | “Am I looking at the right edition/book?” | Duplicate or incomplete catalog records | Canonical book identity and clear metadata |
| Review scan | Reads posts from other readers | “What did people like or dislike?” | Reviews are unstructured or too brief | Show review context and reader identity |
| Taste check | Looks for opinions from readers with similar tastes | “Do people who like what I like recommend it?” | Similarity score may be opaque | Explain shared genres/books where possible |
| Expectation check | Reviews expectation-match feedback | “Did it deliver what its promotion promised?” | Users confuse expectation match with enjoyment | Label these as separate questions and signals |
| Decision | Saves the book or follows an external purchase link | “Do I want to read or buy it?” | Too much friction between evaluation and action | Clear Want to Read and retailer handoff |

**Success signals:** search-to-book-view rate, review engagement, expectation-rating views, save rate, retailer-link clicks.

## Journey 3 — Publish a book post or review

**User goal:** Share a reading experience that helps other readers.

| Stage | User action | User question / thought | Potential friction | Product opportunity |
|---|---|---|---|---|
| Start | Selects Create from navigation or a book page | “Can I share this quickly?” | Unclear post types | Offer clear Review, Recommendation and Reaction choices |
| Compose | Selects a book and writes their post | “What should I include?” | Blank-page anxiety | Lightweight prompts; optional image |
| Rate | Answers the expectation-match question for a review | “What exactly am I rating?” | Confusion with star rating or enjoyment | Explain the scale and keep it distinct |
| Preview | Reviews the post | “Will readers understand my point?” | Missing book context | Preview book card and review together |
| Publish | Publishes the post | “Where will this appear?” | Unclear visibility | Explain feed and book-page placement |
| Engage | Receives reactions or comments | “Did this help anyone?” | Low early engagement | Relevant distribution and respectful notifications |

**Success signals:** post-start-to-publish conversion, review completion rate, expectation-rating completion, useful interactions per post.

## Journey 4 — Build a trusted reader network

**User goal:** Follow readers whose preferences make their recommendations useful.

| Stage | User action | User question / thought | Potential friction | Product opportunity |
|---|---|---|---|---|
| Discovery | Opens suggested readers | “Why am I seeing this person?” | Recommendations feel arbitrary | Show shared genres or books |
| Evaluation | Visits a reader profile | “Do we have similar taste?” | Profile lacks enough reading context | Show public shelves and recent book posts |
| Follow | Follows the reader | “Will their posts improve my feed?” | No clear consequence | Confirm follow and explain feed effect |
| Feed | Sees posts from followed readers | “Is this more relevant?” | Too many posts or repeated content | Ranking, controls and feed diversity |
| Refinement | Follows or unfollows more readers | “Can I shape my discovery?” | Recommendations don't adapt | Use explicit follow and feedback signals |

**Success signals:** suggested-reader profile visits, follow conversion, followed-feed engagement, unfollow rate.

## Cross-journey product requirements to validate

1. A new user must receive useful discovery before following anyone.
2. A book page must make reader opinions easy to scan.
3. Expectation match and enjoyment must not be conflated.
4. The product must show rating counts and avoid implying confidence from tiny samples.
5. Users should understand why a reader or book is recommended.
6. External purchase is a handoff; Perch does not own checkout or fulfilment in Phase 1.

## Research questions

- Where do readers currently discover books?
- What makes a book recommendation credible?
- How do readers decide whether an online review is useful?
- Would readers answer an expectation-match question when posting?
- Would readers use other readers' taste profiles to decide what to read?
- What would make readers return to a dedicated book platform?

## Open decisions

- Is the first feed primarily followed-reader content, discovery content, or a blend?
- Is the expectation-match question required for every review, or only for a specific review type?
- Is an enjoyment rating also needed?
- Are public shelves visible by default?
- Are reading clubs in the first MVP or a later Phase 1 release?
