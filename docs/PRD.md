# Perch

**Status:** ER diagram and PRD done. User research and prototype in progress.

Perch is a dedicated social space for books, built around how people already use social platforms. Readers discover books through other readers instead of relying primarily on promotion feeds and anonymous marketplace reviews.

## The idea

- A book-first social platform: a feed of books and what readers think of them.
- Discovery through readers you trust, not paid promotion or anonymous marketplace reviews.
- Easy creation and publishing support for writers, helping new voices reach readers directly.
- A club for budding writers, with outreach to educational institutions for support and evaluation.
- Tie-ups with publishing houses for distribution. Buying can still happen through external retailers.

### Where it came from

Instagram promotions led to a few books that were not up to the mark. Checking Amazon and Google reviews did not prevent it. Reading *Yellowface* raised the question of how much PR shapes what reaches the shelf, and no existing product seemed to play this role.

## Build order

1. **Readers first** — establish reader discovery, trust, and engagement.
2. **Writers next** — introduce publishing and feedback capabilities once a reader base exists.
3. **Publishing-house distribution later** — explore publisher partnerships after Perch has an established reader base.

## End users

| User | Who they are | What they want from Perch |
|---|---|---|
| Reader | Came to books through social media. Reads around 15 physical books a year. Hears about books on Instagram, then friends, then bookstore bestseller tables. Buys on Amazon or in a bookstore. | Find books they will actually like, before paying for them. |
| Budding writer | Writing something and wants readers and feedback. | Create, publish, get evaluated, and find an audience. |
| Educational institution | Teaches or supports aspiring writers. | A place to support and evaluate student writers. |
| Publishing house | Publishes and distributes books. | Reach readers through a trusted channel. |

## Platform

Perch is a **desktop-first responsive web application**.

The primary experience is designed for desktop and laptop browsers, with responsive support for tablet and mobile browsers. The product is not currently planned as a native mobile application.

## Documentation

| Document | Purpose |
|---|---|
| [Product requirements](docs/product/prd.md) | Product problem, goals, requirements, scope, and success measures |
| [User journey maps](docs/product/user-journey-maps.md) | Reader journeys, actions, friction points, and opportunities |
| [Information architecture](docs/product/information-architecture.md) | Pages, navigation, and content hierarchy |
| [Web experience principles](docs/product/web-experience-principles.md) | Desktop-first layout and responsive behaviour |
| [Use-case diagrams](docs/architecture/use-case-diagram.md) | Actors and their use cases across all three phases |
| [Component diagram](docs/architecture/component-diagram.md) | Logical system components and their responsibilities |
| [Domain model](docs/architecture/domain-model.md) | Core entities, relationships, and domain rules |

## Product phases

### Phase 1 — Readers

Establish the reader experience and validate the core discovery problem.

### Phase 2 — Writers and institutions

Introduce writing publication, reader feedback, writing clubs, institutional programmes, and evaluation.

### Phase 3 — Publishing houses

Explore publisher catalogues, clearly labelled sponsored promotions, reader reception insights, writer discovery, and distribution partnerships.

## Current focus

- Validate the reader discovery problem through user research.
- Refine the Phase 1 scope.
- Develop and test the web prototype.
- Resolve open product and technical decisions before implementation.

---

**Note:** Perch is currently a concept in validation and prototyping. The later phases describe the intended direction, not committed implementation scope.
