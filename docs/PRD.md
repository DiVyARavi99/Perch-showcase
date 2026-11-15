# Perch — Product Requirements Document (PRD)

**Document status:** Draft v0.2  
**Product status:** Concept validation and prototype in progress  
**Platform:** Desktop-first responsive web application  
**Initial release:** Phase 1 — Readers  
**Owner:** Product / Engineering

---

# 1. Product Overview

## 1.1 Product summary

Perch is a dedicated social space for books, built around how people already use social platforms.

Readers discover books through other readers instead of relying primarily on promotion feeds and anonymous marketplace reviews.

The platform brings together book discovery, reader opinions, taste-based connections, and reading activity in a social feed experience.

Perch will eventually expand to support budding writers, educational institutions, and publishing houses. However, the initial product will focus on establishing a meaningful reader community before expanding into the writing and publishing ecosystem.

## 1.2 Problem statement

Readers frequently discover books through social media promotions, influencers, and bestseller recommendations.

However, promotional content does not always reflect the actual reading experience.

Existing review platforms such as Amazon and Google provide ratings and reviews, but they do not necessarily help readers understand whether a book will match their individual tastes or whether it delivered what its promotion promised.

Readers need a way to:

- Discover books through people whose reading preferences they trust.
- Understand how a book was received by readers with similar tastes.
- Evaluate whether a book matched the expectations created by its promotion.
- Make better-informed purchasing decisions before spending money.

**Core problem:** Readers lack a trusted, reader-driven discovery platform that helps them decide whether a book is actually worth reading before buying it.

## 1.3 Product origin

Instagram promotions led to several disappointing book purchases. Checking Amazon and Google reviews did not always prevent this.

Reading *Yellowface* raised a further question: how much does PR influence what reaches readers and bookstore shelves?

Perch explores an alternative: a platform where readers can discover books through other readers, while promotional content remains transparent.

## 1.4 Product vision

Build a book-first social platform where reader experiences drive discovery, emerging writers find an audience, and publishing houses reach readers transparently.

## 1.5 Product principles

1. **Reader-first discovery:** Recommendations should be grounded in reader experiences, not solely promotional activity.
2. **Trust through context:** Opinions from readers with similar tastes should be distinguishable from general ratings.
3. **Transparency:** Sponsored promotions must be clearly labelled.
4. **Expectation versus experience:** A book's enjoyment rating and its expectation-match rating are separate signals.
5. **Progressive expansion:** Establish the reader community before introducing writer and publisher ecosystems.
6. **External purchasing:** Perch facilitates discovery and directs readers to retailers rather than becoming a book-selling or fulfilment platform by default.

---

# 2. Target Users and Actors

Perch has four actor groups across its planned product lifecycle.

| Actor | Description | Primary need |
|---|---|---|
| Reader | Discovers books through social media, friends, and bookstore recommendations. Reads approximately 15 physical books annually and purchases through Amazon or bookstores. | Find books they will actually like before paying for them. |
| Budding writer | An aspiring writer looking for an audience, feedback, and opportunities to improve. | Create, publish, receive feedback, and build an audience. |
| Educational institution | An organisation supporting aspiring writers through programmes, mentorship, or evaluation. | Support and evaluate student writers. |
| Publishing house | An organisation publishing and distributing books. | Reach readers through a trusted channel and discover emerging writers. |

## 2.1 Primary user: Reader

The reader is the initial target user and the foundation of Perch.

Their primary goal is not simply to find popular books. It is to find books that match their preferences and expectations.

## 2.2 Secondary users

Budding writers, educational institutions, and publishing houses are future user groups.

Their capabilities will be introduced in later phases, subject to evidence that the reader community and core discovery experience are working.

---

# 3. Product Strategy and Phases

Perch will be developed in three progressive phases.

## Phase 1 — Readers

**Objective:** Establish reader-driven book discovery and build a trusted reader community.

Core capabilities:

- Social feed for books and reader posts.
- Book discovery and book detail pages.
- Reader reviews, reactions, and recommendations.
- Expectation-match ratings.
- Reader following and taste-based discovery.
- Reading shelves.
- External purchasing links.
- Reading clubs.

Phase 1 is the initial implementation focus.

## Phase 2 — Writers and educational institutions

**Objective:** Enable emerging writers to publish their work, receive feedback, and build an audience.

Writer capabilities:

- Create and publish writing, either as complete works or chapters.
- Receive reader feedback.
- Submit work for institutional or mentor evaluation.
- Join writers clubs.
- Build a following.
- View engagement and reader response.

Institution capabilities:

- Create programmes and cohorts.
- Evaluate submitted writing against a rubric.
- Provide structured mentorship and feedback.
- Conduct showcases and competitions.
- Recognise emerging writers.

**Expansion condition:** Evidence that a meaningful share of active readers also write and that the reader community can support a writing ecosystem.

## Phase 3 — Publishing houses and distribution

**Objective:** Establish transparent publisher participation and explore distribution partnerships.

Publisher capabilities:

- Create verified publisher profiles.
- List catalogues and launch book pages.
- Distribute books to readers through Perch.
- Run clearly labelled sponsored promotions.
- Access reader reception insights.
- Discover emerging writers.

**Expansion condition:** An established reader base and evidence that publisher participation adds value without compromising reader trust.

---

# 4. Product Goals and Success Metrics

## 4.1 Product goals

| Goal | Intended outcome |
|---|---|
| Improve book discovery | Readers discover relevant books beyond bestseller lists and paid promotions. |
| Build reader trust | Readers use opinions from people with similar tastes to evaluate books. |
| Improve purchase confidence | Readers can assess a book's actual reception before buying it. |
| Encourage participation | Readers contribute reviews, reactions, recommendations, and reading activity. |
| Build a reader network | Readers follow other readers based on shared reading preferences. |

## 4.2 Success metrics

The following are proposed measurement areas. Numerical targets should be established after baseline research and prototype testing.

| Metric | What it measures |
|---|---|
| Activation rate | Percentage of registered users who complete onboarding and engage with a book or post. |
| Discovery engagement | Book-detail views and meaningful interactions originating from discovery surfaces. |
| Review contribution rate | Percentage of active readers who publish at least one book-related post or review. |
| Shelf adoption | Percentage of active readers maintaining at least one reading shelf entry. |
| Follow conversion | Percentage of readers who follow at least one other reader. |
| Similar-taste discovery engagement | Engagement with opinions from readers identified as having similar tastes. |
| Expectation-match participation | Percentage of eligible book posts with an expectation-match rating. |
| Return rate | Readers returning to Perch over defined time periods. |
| External purchase-link engagement | Click-throughs to retailer links. |

### Primary product success indicator

**Meaningful reader discovery:** The extent to which readers use Perch to discover books, evaluate reader experiences, and make informed reading or purchasing decisions.

The precise north-star metric and its calculation remain to be validated.

---

# 5. MVP Scope — Phase 1

## 5.1 In scope

| Capability | Description | Related use cases |
|---|---|---|
| Reader onboarding | Account creation and basic reader profile setup. | Supporting capability |
| Home feed | Browse books and reader-generated posts. | R1 |
| Book discovery | Search and explore available book records. | R1, R2 |
| Book detail page | View book information, reader opinions, and relevant ratings. | R2 |
| Reader posts | Publish reactions, reviews, and recommendations. | R3 |
| Expectation-match rating | Rate how a book matched the expectations created by its promotion. | R4 |
| Reader following | Follow readers with similar reading tastes. | R5 |
| Reading shelves | Maintain want-to-read, currently-reading, and read lists. | R6 |
| External purchase links | Navigate to Amazon or bookstore listings. | R7 |
| Reading clubs | Join and participate in book discussions. | R8 |
| Reader profiles | View reader information, activity, and reading preferences. | Supporting capability |
| Notifications | Receive relevant activity updates. | Supporting capability |

R9, reading and reacting to writing published on Perch, is a Phase 2 crossover capability and is not part of the initial MVP.

## 5.2 Out of scope for Phase 1

- Native mobile applications.
- Writer publishing and chapter management.
- Institutional accounts and evaluation workflows.
- Publisher accounts and verified catalogues.
- Paid or sponsored promotions.
- In-platform book purchasing and fulfilment.
- Advanced AI-based recommendation systems.
- Publisher analytics and writer scouting.

## 5.3 MVP boundaries

The first release should validate the reader discovery problem, not attempt to build the entire future Perch ecosystem.

The product should provide useful discovery even when a new reader has not followed anyone yet.

Initial discovery can use available book information, reader activity, explicit preferences, and popular or relevant community content. More sophisticated personalisation can evolve after sufficient data is available.

---

# 6. Functional Requirements

The following requirements define expected product behaviour for Phase 1.

## 6.1 Reader onboarding and profile

**FR-01 — Account creation**

The system shall allow a reader to register and access a personal Perch account.

**FR-02 — Reader profile**

The system shall allow readers to create and manage a profile containing basic information and reading-related preferences.

**FR-03 — Profile visibility**

The system shall support appropriate profile visibility controls. Exact privacy defaults are to be finalised.

## 6.2 Feed and discovery

**FR-04 — Reader feed**

The system shall provide a feed containing books and reader-generated posts.

**FR-05 — Feed content**

The feed shall support relevant content such as reader reviews, reactions, recommendations, and book-related activity.

**FR-06 — Book discovery**

The system shall allow readers to search for and discover books.

**FR-07 — Book detail**

The system shall provide a dedicated page for each book containing available metadata and reader-generated opinions.

**FR-08 — New-user discovery**

The system shall provide useful discovery content to readers who have not yet followed other users.

## 6.3 Reviews and reader contributions

**FR-09 — Create book posts**

The system shall allow readers to publish a reaction, review, or recommendation associated with a book.

**FR-10 — Expectation-match rating**

The system shall ask readers to rate how well a book matched the expectations created by its promotion when they publish a book post.

This rating shall represent expectation fulfilment, not simply enjoyment.

**FR-11 — Separate rating dimensions**

The system shall distinguish the reader's enjoyment or opinion of a book from its expectation-match rating.

**FR-12 — View reader opinions**

The system shall display relevant reader posts and opinions on book detail pages.

## 6.4 Social graph and taste matching

**FR-13 — Follow readers**

The system shall allow readers to follow other readers.

**FR-14 — Similar-taste discovery**

The system shall support the identification and discovery of readers with similar reading preferences.

**FR-15 — Reader context**

Where sufficient data exists, the system shall help readers distinguish opinions from similar-taste readers from general reader opinions.

## 6.5 Reading shelves

**FR-16 — Shelf management**

The system shall allow readers to organise books into:

- Want to read.
- Currently reading.
- Read.

**FR-17 — Shelf updates**

Readers shall be able to add books to shelves and update their reading status.

## 6.6 External purchasing

**FR-18 — Retailer links**

The system shall provide external purchasing links to Amazon or supported bookstores when available.

**FR-19 — External handoff**

Selecting a purchase link shall redirect the reader to the relevant external retailer.

Perch shall not process book payments or fulfil orders as part of Phase 1.

## 6.7 Reading clubs and engagement

**FR-20 — Reading clubs**

The system shall allow readers to discover and join reading clubs.

**FR-21 — Club discussions**

The system shall support book-related discussions within reading clubs.

**FR-22 — Notifications**

The system shall notify readers about relevant activity, such as interactions with their posts, follows, and club activity.

---

# 7. User Experience and Platform Requirements

## 7.1 Platform decision

Perch shall be developed as a **desktop-first responsive web application**.

The primary experience will target desktop and laptop browsers. Tablet and mobile browsers will be supported through responsive layouts.

Native mobile applications are not part of the current scope.

## 7.2 Core navigation

The desktop application shall provide persistent navigation for major product areas.

Expected navigation areas:

- Home.
- Discover.
- My Shelves.
- Reading Clubs.
- Notifications.
- Profile.
- Create Post.

A contextual right-hand panel may be used for recommendations, suggested readers, or relevant discovery content.

## 7.3 Key pages

| Page | Primary purpose |
|---|---|
| Home | Browse the reader feed. |
| Discover | Search and explore books and readers. |
| Book Detail | Evaluate a book using metadata and reader opinions. |
| Reader Profile | Explore a reader's activity and shelves. |
| My Shelves | Manage reading lists. |
| Create Post | Publish a book reaction, review, or recommendation. |
| Reading Club | Participate in book discussions. |
| Notifications | View relevant account activity. |

## 7.4 Responsive behaviour

- Desktop: Persistent sidebar, central content area, optional right rail.
- Smaller desktop: Compact or collapsible sidebar.
- Tablet: Reduced navigation and single-column content where appropriate.
- Mobile browser: Compact navigation and single-column layout.

## 7.5 UX principles

- Discovery should be easy to navigate.
- Book information and reader opinions should be easy to distinguish.
- Expectation-match ratings should have clear explanations.
- Sponsored content, when introduced, must be visually distinguishable.
- Important interactions must not depend exclusively on hover.
- Pages should have stable, shareable URLs and support browser navigation.

---

# 8. Non-Functional Requirements

These requirements define quality expectations rather than specific technology choices.

| Category | Requirement |
|---|---|
| Performance | Core pages and interactions should load and respond within acceptable web performance thresholds. Targets will be established before implementation. |
| Scalability | The system should support growth in readers, books, posts, and interactions without requiring a complete architectural redesign. |
| Security | Authentication, authorisation, and protection of user data must be implemented. |
| Privacy | Users should have appropriate control over personal information and profile visibility. |
| Accessibility | The web application should support keyboard navigation, readable contrast, semantic structure, and accessible controls. |
| Responsiveness | Core experiences should work across desktop, tablet, and mobile browser sizes. |
| Reliability | Core discovery, reading, and posting workflows should handle failures gracefully. |
| Maintainability | Product components should have clear responsibilities and documented interfaces. |
| Moderation | Users should be able to report inappropriate content, and the platform should support moderation workflows. |
| Data integrity | Book records, user posts, shelf entries, and ratings should remain consistent across relevant views. |

---

# 9. Trust, Transparency, and Moderation

Trust is central to Perch's product positioning.

## 9.1 Expectation-match transparency

The expectation-match rating must not be presented as another generic star rating.

It should communicate whether a book delivered what the reader expected based on the promotion or recommendation that influenced their interest.

The rating should remain distinct from the reader's enjoyment of the book.

## 9.2 Reader-generated content

Reader reviews and recommendations should be clearly attributed to their authors, subject to privacy settings.

The platform should provide mechanisms to report inappropriate, misleading, or abusive content.

## 9.3 Sponsored content

Sponsored promotions are planned for Phase 3.

When introduced:

- Sponsored content must be explicitly labelled.
- Paid promotion must not be disguised as organic reader opinion.
- Reader ratings and reviews must remain distinct from publisher-provided promotional material.

## 9.4 Moderation

The platform should provide:

- Content reporting.
- Basic moderation workflows.
- Account and content enforcement mechanisms.
- Clear community guidelines.

Detailed moderation policies and escalation processes will be defined before public launch.

---

# 10. External Integrations and Dependencies

The following are potential integration areas. Final providers and implementation choices are not yet decided.

| Integration | Purpose | Phase |
|---|---|---|
| Book metadata provider | Retrieve book details, authors, covers, and identifiers. | Phase 1 |
| External retailers | Redirect readers to book purchasing pages. | Phase 1 |
| Identity provider | Support authentication where appropriate. | Phase 1 |
| Email/notification provider | Deliver account and activity notifications. | Phase 1 |
| Publisher catalogue integration | Support publisher book listings. | Phase 3 |

Potential book metadata sources include Open Library and Google Books. Their coverage, terms, and licensing requirements must be evaluated before selection.

---

# 11. Dependencies and Risks

| Risk or dependency | Potential impact | Mitigation / consideration |
|---|---|---|
| Insufficient reader activity | Feed may feel empty and taste matching may be weak. | Validate onboarding and seed useful discovery content. |
| Cold-start problem | New readers have limited social and preference data. | Provide useful discovery without requiring follows. |
| Low review contribution | Book pages may lack meaningful reader opinions. | Make posting straightforward and encourage useful contributions. |
| Unclear expectation-match rating | Readers may interpret it as an ordinary rating. | Explain the rating dimension and test the wording with users. |
| Book metadata coverage | Missing or duplicate records may hurt discovery. | Evaluate providers and define book identity and deduplication rules. |
| Sponsored content conflicts | Commercial participation may weaken trust. | Require explicit labelling and separate promotional content from organic reviews. |
| Scope expansion | Later-phase capabilities may delay the reader MVP. | Maintain strict phase boundaries. |
| Content abuse | User-generated content may create moderation challenges. | Establish reporting and moderation processes before launch. |

---

# 12. Acceptance Criteria — Phase 1

The MVP can be considered functionally ready for initial validation when the following conditions are met.

| Area | Acceptance criteria |
|---|---|
| Onboarding | A reader can register, access an account, and create a basic profile. |
| Home feed | A reader can view a feed of book-related posts. |
| Discovery | A reader can search for and open a book detail page. |
| Book details | Available book metadata and reader opinions are displayed in a clear structure. |
| Reader posts | A reader can create and publish a book-related post. |
| Expectation match | A reader can submit an expectation-match rating when publishing a book post. |
| Rating distinction | The interface clearly distinguishes expectation match from enjoyment or general opinion. |
| Social graph | A reader can follow another reader and view relevant reader activity. |
| Shelves | A reader can add a book to a shelf and update its reading status. |
| Retailer handoff | A reader can follow an available external purchase link. |
| Reading clubs | A reader can discover, join, and participate in a reading club. |
| Notifications | Relevant account activity can be surfaced to the reader. |
| Responsive web | Core workflows are usable on desktop, tablet, and mobile browser layouts. |
| Moderation | A reader can report inappropriate content. |

These criteria establish functional readiness. Performance, accessibility, security, and reliability thresholds must also be verified before release.

---

# 13. Open Product Decisions

The following decisions need validation or explicit agreement before implementation.

| ID | Decision | Why it matters |
|---|---|---|
| D01 | What exactly qualifies as the expectation source for R4? | A reader may discover a book through a friend, social media, a publisher, or an organic recommendation. |
| D02 | Should expectation-match ratings support a not-applicable option? | Not every reader will have encountered a specific promotion. |
| D03 | How should similar-taste readers be identified initially? | Determines whether the first version uses explicit preferences, shelf overlap, follows, or a combination. |
| D04 | What is the initial feed-ranking strategy? | Determines discovery quality and cold-start behaviour. |
| D05 | Should reading clubs be included in the first public MVP or introduced after core discovery validation? | Clubs introduce additional social and moderation complexity. |
| D06 | Which book metadata provider should be used? | Affects book coverage, quality, licensing, and duplicate records. |
| D07 | Should profiles and book pages be publicly accessible without login? | Affects sharing, discovery, and privacy. |
| D08 | What are the default privacy settings for reader profiles, shelves, and activity? | Affects user trust and visibility. |
| D09 | What is the initial moderation model? | Determines operational responsibilities for user-generated content. |
| D10 | What should the primary product success metric be? | Requires validation against actual reader behaviour. |

---

# 14. Roadmap and Next Steps

## Current stage — Validation and prototype

- Validate the reader discovery problem with target users.
- Test the expectation-match rating concept.
- Validate the core reader journeys.
- Review the Stitch prototype against the information architecture.
- Resolve critical Phase 1 product decisions.

## Before development

- Finalise Phase 1 scope.
- Convert functional requirements into an implementation backlog.
- Define detailed acceptance criteria for individual features.
- Finalise domain entities and relationships.
- Decide the initial technical architecture.
- Establish baseline analytics and instrumentation requirements.

## Phase 1 — Build and validate

Build the reader experience and validate whether Perch improves book discovery and reader confidence.

## Phase 2 — Expand

Introduce writing and institutional capabilities when the reader ecosystem supports them.

## Phase 3 — Partner

Introduce publisher participation and distribution opportunities while protecting reader trust.

---

# 15. Related Documentation

This PRD defines the product problem, strategy, requirements, scope, and success criteria.

Detailed supporting documentation is maintained separately to avoid duplicating information.

| Document | Responsibility |
|---|---|
| [User journey maps](user-journey-maps.md) | Step-by-step user journeys, friction points, and opportunities. |
| [Information architecture](information-architecture.md) | Page hierarchy, navigation, and content organisation. |
| [Web experience principles](web-experience-principles.md) | Desktop-first responsive web experience. |
| [Use-case diagrams](../architecture/use-case-diagram.md) | Complete actor capabilities and use-case relationships. |
| [Component diagram](../architecture/component-diagram.md) | Logical system components and their responsibilities. |
| [Domain model](../architecture/domain-model.md) | Core entities, relationships, and domain rules. |

---

**Document note:** This PRD is a working product specification. Requirements and assumptions may change based on user research, prototype testing, and validation. Phase 2 and Phase 3 capabilities are part of the product vision, not commitments for the initial release.
