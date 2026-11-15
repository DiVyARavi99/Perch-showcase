# Perch — Use Case Diagram

## 1. Overview

Perch has four primary actor groups:

1. **Reader** — discovers books through other readers, shares opinions and builds a reading network.
2. **Budding Writer** — publishes writing, receives feedback and builds an audience.
3. **Educational Institution** — supports, evaluates and showcases emerging writers.
4. **Publishing House** — manages verified book catalogues, promotes books and discovers emerging writers.

The product is planned across three phases:

- Phase 1: Reader ecosystem.
- Phase 2: Writer and institution ecosystem.
- Phase 3: Publisher ecosystem.

## 2. Reader Use Cases — Phase 1

```mermaid
flowchart LR
    R((Reader))

    subgraph PERCH["Perch — Reader Ecosystem"]
        UC1[Browse book feed]
        UC2[Discover books]
        UC3[View book details]
        UC4[Read reader reviews]
        UC5[View similar-taste readers' opinions]
        UC6[Evaluate expectation match]
        UC7[Create book post or review]
        UC8[Rate reading experience]
        UC9[Follow readers]
        UC10[Manage reading shelves]
        UC11[Access external purchase links]
        UC12[Join reading clubs]
        UC13[Interact with posts]
        UC14[Manage profile]
        UC15[Receive notifications]
    end

    R --> UC1
    R --> UC2
    R --> UC3
    R --> UC4
    R --> UC5
    R --> UC6
    R --> UC7
    R --> UC8
    R --> UC9
    R --> UC10
    R --> UC11
    R --> UC12
    R --> UC13
    R --> UC14
    R --> UC15

    UC7 -.->|includes| UC8
    UC3 -.->|includes| UC4
    UC4 -.->|may include| UC5
    UC3 -.->|may include| UC6
```

### Reader use-case descriptions

| ID | Use case | Description |
|---|---|---|
| R1 | Browse feed | View book-related posts from readers |
| R2 | Discover books | Search and explore books by genre or interest |
| R3 | View book details | Access book information and reader reception |
| R4 | Read reviews | Evaluate opinions shared by readers |
| R5 | Similar-taste opinions | Find reviews from readers with overlapping reading preferences |
| R6 | Expectation match | Understand whether a book met reader expectations |
| R7 | Create post | Share a reaction, review or recommendation |
| R8 | Rate experience | Record enjoyment and expectation match separately |
| R9 | Follow readers | Build a network around reading interests |
| R10 | Manage shelves | Organise books into Want to Read, Currently Reading and Read |
| R11 | External purchase | Navigate to external retailer pages |
| R12 | Reading clubs | Join and participate in book communities |
| R13 | Interact | React to and comment on posts |
| R14 | Manage profile | Maintain reader identity and public reading activity |
| R15 | Notifications | Receive relevant social and community updates |

## 3. Budding Writer Use Cases — Phase 2

```mermaid
flowchart LR
    W((Budding Writer))

    subgraph PERCH["Perch — Writer Ecosystem"]
        W1[Create writing work]
        W2[Publish chapters or complete work]
        W3[Receive reader feedback]
        W4[Submit work for evaluation]
        W5[Participate in writers clubs]
        W6[Build reader following]
        W7[View engagement metrics]
        W8[Manage published works]
    end

    W --> W1
    W --> W2
    W --> W3
    W --> W4
    W --> W5
    W --> W6
    W --> W7
    W --> W8
```

## 4. Educational Institution Use Cases — Phase 2

```mermaid
flowchart LR
    I((Educational Institution))

    subgraph PERCH["Perch — Institution Ecosystem"]
        I1[Create writing programmes]
        I2[Manage cohorts]
        I3[Collect writing submissions]
        I4[Evaluate submissions]
        I5[Provide structured feedback]
        I6[Mentor writers]
        I7[Organise showcases and competitions]
        I8[Recognise emerging writers]
    end

    I --> I1
    I --> I2
    I --> I3
    I --> I4
    I --> I5
    I --> I6
    I --> I7
    I --> I8
```

## 5. Publishing House Use Cases — Phase 3

```mermaid
flowchart LR
    P((Publishing House))

    subgraph PERCH["Perch — Publisher Ecosystem"]
        P1[Manage verified publisher profile]
        P2[Manage book catalogue]
        P3[Create sponsored promotions]
        P4[View reader reception]
        P5[Discover emerging writers]
        P6[Access book engagement insights]
        P7[Link books to external retailers]
    end

    P --> P1
    P --> P2
    P --> P3
    P --> P4
    P --> P5
    P --> P6
    P --> P7
```

## 6. Scope Boundaries

| Phase | Actor | Scope |
|---|---|---|
| Phase 1 | Reader | Book discovery, reviews, shelves, social interactions and reading clubs |
| Phase 2 | Budding Writer | Writing publication, feedback and audience development |
| Phase 2 | Educational Institution | Programmes, evaluation, mentoring and showcases |
| Phase 3 | Publishing House | Verified catalogues, promotions, reader analytics and writer discovery |

**Important:** The diagrams describe intended product capabilities, not a commitment to implement every use case in the first release. The Phase 1 MVP must be prioritised separately.

