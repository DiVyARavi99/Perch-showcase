# Perch

**Status: concept. No code yet. User research in planning.**

A dedicated social space for books, built like Instagram. Readers discover books through other readers instead of through promotion feeds and marketplace reviews.

## The idea

- A book-first social platform: a feed of books and what readers think of them, in the format people already scroll.
- Discovery through readers you trust, not through paid promotion or anonymous marketplace reviews.
- Easy creation and publishing support for writers, so new voices reach readers directly.
- A club for budding writers, with outreach to educational institutions for support and evaluation of aspiring writers.
- Tie-ups with publishing houses for distribution. Not against Amazon; buying can still happen there.

### Where it came from

Instagram promotions led to a few books that were not up to the mark. Checking Amazon and Google reviews did not prevent it. Reading *Yellowface* raised the question of how much PR shapes what reaches the shelf, and no existing product seemed to play this role.

### Order of build

1. Readers first.
2. Writers next, once the reader base exists.
3. Publishing-house distribution after that.

## End users

| User | Who they are | What they want from Perch |
|---|---|---|
| Reader | Came to books through social media. Reads around 15 physical books a year. Hears about books on Instagram, then friends, then bookstore bestseller tables. Buys on Amazon or in a bookstore. | Find books they will actually like, before paying for them. |
| Budding writer | Writing something and wants readers and feedback. | Create, publish, get evaluated, find an audience. |
| Educational institution | Teaches or supports aspiring writers. | A place to support and evaluate student writers. |
| Publishing house | Publishes and distributes books. | Reach readers through a trusted channel. |

## System overview

All four actors against the system boundary. Core use cases only; the full set per actor follows.

```mermaid
flowchart LR
  Reader["Reader"]
  Writer["Budding writer"]
  Inst["Educational institution"]
  Pub["Publishing house"]

  subgraph Perch
    direction TB
    subgraph P1["Phase 1: readers"]
      R1(["Browse a feed of books and reader posts"])
      R2(["Check what readers think before buying"])
      R3(["Post about a book"])
      R5(["Follow readers with similar taste"])
      R6(["Track books: want to read, reading, read"])
      R7(["Buy through a link to Amazon or a bookstore"])
    end
    subgraph P2["Phase 2: writers"]
      W1(["Create and publish writing"])
      W2(["Get feedback from readers"])
      W4(["Join a writers club"])
      I2(["Evaluate submitted writing"])
    end
    subgraph P3["Phase 3: distribution"]
      P2x(["Distribute books through Perch"])
    end
    P1 ~~~ P2
    P2 ~~~ P3
  end

  Reader --> R1
  Reader --> R2
  Reader --> R3
  Reader --> R5
  Reader --> R6
  Reader --> R7
  Reader -. reads .-> W1
  Writer --> W1
  Writer --> W2
  Writer --> W4
  Inst --> I2
  Pub --> P2x
```

## Use cases by actor

Each diagram shows one actor and everything they can do in the system. Dotted arrows marked «include» are steps that always happen as part of the parent use case.

### Reader

Phase 1. The reader is the wedge; everything here ships first.

```mermaid
flowchart LR
  Reader["Reader"]

  subgraph Perch
    direction TB
    R1(["R1 Browse a feed of books and reader posts"])
    R2(["R2 Check what readers think of a book before buying"])
    R2a(["R2a See the verdict from readers with similar taste"])
    R2b(["R2b See how the book matched expectations, not just stars"])
    R3(["R3 Post about a book: reaction, review, recommendation"])
    R4(["R4 Rate how a book matched what the promotion promised"])
    R5(["R5 Follow readers with similar taste"])
    R6(["R6 Track books: want to read, reading, read"])
    R7(["R7 Buy through a link to Amazon or a bookstore"])
    R8(["R8 Join a reading club and discuss a book"])
    R9(["R9 Read and react to writing published on Perch"])
  end

  Reader --> R1
  Reader --> R2
  Reader --> R3
  Reader --> R4
  Reader --> R5
  Reader --> R6
  Reader --> R7
  Reader --> R8
  Reader --> R9
  R2 -. «include» .-> R2a
  R2 -. «include» .-> R2b
  R2 -. leads to .-> R7
  R3 -. «include» .-> R4
```

| ID | Use case | Notes |
|---|---|---|
| R1 | Browse a feed of books and reader posts | The Instagram-shaped surface |
| R2 | Check what readers think of a book before buying it | The core job. Replaces the Amazon and Google review check |
| R2a | See the verdict from readers with similar taste | Always part of R2. Needs R5 data |
| R2b | See how the book matched expectations, not just stars | Always part of R2. Fed by R4 |
| R3 | Post about a book | Reaction, review, or recommendation |
| R4 | Rate how a book matched what the promotion promised | Always asked when posting. This is the signal Amazon does not have |
| R5 | Follow readers with similar taste | Builds the trust graph |
| R6 | Track books as want to read, reading, or read | Shelf |
| R7 | Buy through a link to Amazon or a bookstore | Perch does not sell; it hands off |
| R8 | Join a reading club and discuss a book | Group reading |
| R9 | Read and react to writing published on Perch | Phase 2 crossover: readers are the audience for writers |

### Budding writer

Phase 2. Gated on evidence that a meaningful share of active readers also write.

```mermaid
flowchart LR
  Writer["Budding writer"]

  subgraph Perch
    direction TB
    W1(["W1 Create and publish writing, whole or in chapters"])
    W2(["W2 Get feedback from readers"])
    W3(["W3 Submit work for evaluation by an institution or mentor"])
    W4(["W4 Join a writers club"])
    W5(["W5 Build a following"])
    W6(["W6 See how readers respond: reads, saves, reactions"])
  end

  Writer --> W1
  Writer --> W2
  Writer --> W3
  Writer --> W4
  Writer --> W5
  Writer --> W6
  W1 -. leads to .-> W2
  W1 -. leads to .-> W6
```

| ID | Use case | Notes |
|---|---|---|
| W1 | Create and publish writing, as a whole or in chapters | The publishing tool |
| W2 | Get feedback from readers | Comes from R9 on the reader side |
| W3 | Submit work for evaluation by an institution or mentor | Connects to I2 |
| W4 | Join a writers club | Peer group |
| W5 | Build a following | Same follow graph as readers, R5 |
| W6 | See how readers respond | Reads, saves, reactions on published work |

### Educational institution

Phase 2. An institution is a partner account, not an individual.

```mermaid
flowchart LR
  Inst["Educational institution"]

  subgraph Perch
    direction TB
    I1(["I1 Run a program or cohort for aspiring writers"])
    I2(["I2 Evaluate submitted writing against a rubric"])
    I3(["I3 Mentor and give structured feedback"])
    I4(["I4 Run showcases or competitions and recognize writers"])
  end

  Inst --> I1
  Inst --> I2
  Inst --> I3
  Inst --> I4
  I1 -. «include» .-> I2
  I1 -. «include» .-> I3
```

| ID | Use case | Notes |
|---|---|---|
| I1 | Run a program or cohort for aspiring writers | A cohort groups writers under the institution |
| I2 | Evaluate submitted writing against a rubric | Receives W3 submissions |
| I3 | Mentor and give structured feedback | Different from reader feedback in W2: structured, attributed |
| I4 | Run showcases or competitions and recognize writers | Recognition shows on the writer's profile |

### Publishing house

Phase 3. Depends on a reader base that does not exist yet.

```mermaid
flowchart LR
  Pub["Publishing house"]

  subgraph Perch
    direction TB
    P1(["P1 List a catalog and launch book pages"])
    P2x(["P2 Distribute books to readers through Perch"])
    P3(["P3 Run promotions that are labeled as sponsored"])
    P4(["P4 See reader reception: expectation-match ratings, reads, saves"])
    P5(["P5 Scout emerging writers from the writing side of Perch"])
  end

  Pub --> P1
  Pub --> P2x
  Pub --> P3
  Pub --> P4
  Pub --> P5
  P1 -. leads to .-> P2x
  P1 -. leads to .-> P4
```

| ID | Use case | Notes |
|---|---|---|
| P1 | List a catalog and launch book pages | Publisher-verified book pages |
| P2 | Distribute books to readers through Perch | Fulfilment still via Amazon or bookstores, R7 |
| P3 | Run promotions that are labeled as sponsored | Promotion is allowed, hiding it is not. This is what makes Perch different from the Instagram feed |
| P4 | See reader reception | Expectation-match ratings from R4, reads, saves |
| P5 | Scout emerging writers | Reads W6 signals. The Yellowface thread, done in the open |

## Component diagram

Responsibilities, not technology choices. Stack is undecided. Phase labels match the build order.

```mermaid
flowchart TB
  subgraph Clients
    Mobile["Mobile app"]
    Web["Web app"]
  end

  subgraph Edge
    API["API gateway and auth"]
  end

  subgraph Core["Core services: Phase 1"]
    Catalog["Book catalog"]
    Feed["Feed"]
    Posts["Posts and ratings"]
    Social["Social graph: follows, clubs"]
    Taste["Taste matching"]
    Shelf["Shelf: want to read, reading, read"]
    Notify["Notifications"]
  end

  subgraph Writing["Writing services: Phase 2"]
    Publish["Writing and publishing"]
    Eval["Feedback and evaluation"]
    Programs["Institution programs"]
  end

  subgraph Dist["Distribution: Phase 3"]
    Portal["Publisher portal"]
  end

  subgraph Data
    DB[("Relational database")]
    Search[("Search index")]
    Media[("Object storage: covers, media")]
    Cache[("Cache")]
    Events[["Event stream"]]
  end

  subgraph External
    BookAPI["Book metadata: Open Library, Google Books"]
    Retail["Amazon and bookstore links"]
    Push["Email and push provider"]
    IdP["Identity provider"]
  end

  Mobile --> API
  Web --> API
  API --> IdP
  API --> Catalog
  API --> Feed
  API --> Posts
  API --> Social
  API --> Shelf
  API --> Publish
  API --> Eval
  API --> Programs
  API --> Portal

  Catalog --> BookAPI
  Catalog --> DB
  Catalog --> Search
  Catalog --> Media

  Posts --> DB
  Posts --> Events
  Shelf --> DB
  Shelf --> Events
  Social --> DB
  Social --> Events

  Events --> Taste
  Events --> Feed
  Events --> Notify
  Taste --> Cache
  Feed --> Cache
  Feed --> Search
  Notify --> Push

  Posts --> Retail

  Publish --> DB
  Publish --> Media
  Publish --> Events
  Eval --> DB
  Programs --> DB

  Portal --> Catalog
  Portal --> Posts
  Portal --> Publish
```

### What each component owns

| Component | Owns | Used by |
|---|---|---|
| API gateway and auth | Routing, sessions, rate limits | All clients |
| Book catalog | Canonical book records, covers, search | R1, R2, R6, P1 |
| Feed | Ranking and assembling what a reader sees | R1 |
| Posts and ratings | Reader posts, expectation-match ratings, buy links | R3, R4, R7, P4 |
| Social graph | Follows, clubs, cohorts | R5, R8, W4, W5, I1 |
| Taste matching | Similar-taste scoring from posts, shelves, follows | R2a, R5 |
| Shelf | Want to read, reading, read | R6 |
| Notifications | Push and email | All actors |
| Writing and publishing | Drafts, chapters, published works | W1, R9 |
| Feedback and evaluation | Reader feedback, rubric evaluations, mentor notes | W2, W3, I2, I3 |
| Institution programs | Cohorts, showcases, competitions, recognition | I1, I4 |
| Publisher portal | Catalog listing, labeled promotions, reception analytics, scouting | P1 to P5 |
| Event stream | Every post, rating, shelf change, follow, publish | Taste matching, Feed, Notifications |

---

Reader use cases R1, R3, R5, and R6 are read off "like Instagram": feed, post, follow, save. R4 and P3 are proposals that follow from the problem statement: the signal that is missing today is whether a book matched its promotion, and promotion itself is fine as long as it is labeled. Edit anything that is not what you meant.
