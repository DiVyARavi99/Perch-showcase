# Perch — Product Requirements Document (PRD) & Product Brief

**Status:** Approved / Release Baseline  
**Document Version:** 1.0  
**Project Ecosystem:** Perch Literary Social & Protocol  
**Target Formats:** Web Application (Primary Desktop Workspace) & Mobile Companion  

---

## 1. Executive Summary & Vision

**Perch** is a book-first literary ecosystem and decentralized publishing protocol designed to replace algorithmic, star-based book discovery with **taste concordance, community-governed marginalia, and verified literary provenance**. 

Unlike conventional book platforms dominated by aggregate star ratings and commercial review bombing, Perch aligns the incentives of four distinct literary stakeholders:
1. **Readers (R1–R9)**: Discover books through trusted literary circles, evaluate reads against calibrated authorial expectation contracts rather than generic star counts, and share rich inline marginalia.
2. **Budding Writers (W1–W6)**: Draft, serialize, and publish manuscripts in whole or serial chapters, solicit targeted inline reader feedback, and build a dedicated literary following.
3. **Educational Institutions & Mentors (I1–I4)**: Host accredited MFA and writing cohorts, grade student manuscripts against structured multi-dimensional rubrics, provide line-level critique, and sponsor juried public competitions.
4. **Publishing Houses & Imprints (P1–P5)**: Register bibliographic catalog records, calibrate authorial expectation baselines, distribute cryptographically watermarked Advance Reader Copies (ARCs) to matched taste cohorts, run transparent sponsored promotions, and scout breakout literary talent directly from the writing ecosystem.

---

## 2. Core Stakeholder Architecture & Use Case Mapping

### Phase 1: Reader Ecosystem (R1–R9)
* **R1 — Feed Browsing**: Chronological, circle-curated feed of books, reader essays, and margin notes without algorithmic dopamine traps.
* **R2 — Pre-Purchase Evaluation**: Multi-dimensional evaluation combining:
  * **R2a — Taste Concordance**: Scores filtered strictly by readers with historically correlated reading preferences.
  * **R2b — Expectation vs. Reality Verdicts**: Reviews weighted against authorial premise contracts (e.g., narrative pacing, prose texture, atmospheric gravity) rather than arbitrary 1–5 star ratings.
* **R3 — Literary Posting**: Publishing thoughtful reviews, book reactions, and curated reading stacks.
* **R4 — Expectation Concordance Rating**: Scoring how faithfully a book matched what its editorial premise and jacket promised.
* **R5 — Taste Match Discovery**: Discovering and following other readers through mathematical reading affinity curves and salon circles.
* **R6 — Reading Tracker & Shelf**: Organizing personal libraries into "Want to Read", "Currently Reading", "Read", and "Living Stacks".
* **R7 — Outbound Independent Purchasing**: Direct affiliate purchase routing supporting independent booksellers (Bookshop.org, Powell’s, direct publisher imprints).
* **R8 — Reading Clubs & Salons**: Synchronous and asynchronous reading rooms featuring live chapter marginalia reels, pacing stats, and salon discussion boards.
* **R9 — Published Works Consumption**: High-fidelity, distraction-free reading canvas featuring Newsreader typography, author-anchored inquiries, and live margin notes.

---

### Phase 2: Writing & Institutional Services (W1–W6, I1–I4)

#### Budding Writers (W1–W6)
* **W1 — Serialization & Chapter Publishing**: Authoring desk supporting whole manuscripts or serial release cadences with custom margin note permissions.
* **W2 — Inline Reader Feedback**: Paragraph-anchored craft inquiries allowing authors to ask targeted questions (e.g., line pacing, dialect plausibility) directly in the text.
* **W3 — Institutional Submission**: Structured intake portal for submitting manuscripts to academic fellowships, MFA cohorts, and mentor critique pools.
* **W4 — Writers Guild & Peer Workshops**: Peer review circles with structured critique rubrics, manuscript swaps, and NDA/embargo governance.
* **W5 — Following & Patron Guilds**: Building a direct reader base with tiered release access (Guild supporters vs. public feeds).
* **W6 — Telemetry & Engagement Analytics**: Quantitative metrics on chapter reads, margin notes volume, drop-off heatmaps, and sentiment tag distribution.

#### Educational Institutions (I1–I4)
* **I1 — Program & Cohort Management**: Partner accounts for MFA workshops, literary foundations, and writing residencies to oversee fellows and curriculum tracks.
* **I2 — Rubric Grading Engine**: Standardized 100-point composite matrix assessing Thematic Depth, Prose Cadence, Narrative Arc, and Worldbuilding against institutional benchmarks.
* **I3 — Structured Mentorship Desk**: Line-by-line editorial annotation desk, faculty diagnostic synthesis generation, and 1:1 salon debrief booking.
* **I4 — Showcase Gallery & Juried Competitions**: Curated public exhibition halls showcasing fellowship medalists, jury citations, and anthology selections.

---

### Phase 3: Distribution & Publisher Portal (P1–P5)

* **P1 — Bibliographic Registry & Book Launch**: Ingestion of edition registry IDs, ISBN-13 barcodes, cloth spine tokens, multi-format releases, and authorial expectation contract calibration.
* **P2 — Targeted ARC Distribution**: Proof pool management with automated SHA-256 dynamic steganographic watermarking, routed exclusively to matched reader taste cohorts.
* **P3 — Transparent Sponsored Promotions**: Publisher campaign launcher with mandatory "Sponsored" transparency disclosure, budget pacing, and shelf-addition ROI.
* **P4 — Reception & Concordance Analytics**: Real-time reader reception tracking measuring expectation concordance against the author's calibrated premise.
* **P5 — Emerging Writer Scouting**: Dedicated discovery funnel to scout top-performing unrepresented writers from Phase 2, review faculty appraisals, and initiate acquisition queries.

---

## 3. Technical Architecture & Data Schemas

### 3.1 Backend Architecture Overview
```
Clients (Desktop Web & Mobile Apps)
  └── Edge API Gateway & Auth
        ├── Core Services (Phase 1)
        │     ├── Book Catalog & Bibliographic Metadata (P1, R7)
        │     ├── Social Graph: Follows, Circles & Salons (R5, R8)
        │     ├── Shelf Tracker & Reading History (R6)
        │     ├── Postings, Marginalia & Concordance Ratings (R1, R3, R4)
        │     ├── Taste Match Matrix Engine (R2a, R5)
        │     └── Notification & Event Dispatcher
        ├── Writing Services (Phase 2)
        │     ├── Manuscript Serialization & Version Engine (W1)
        │     ├── Inline Anchor & Pre-Review Query Broker (W2, W3)
        │     ├── Institutional Programs & Cohort Manager (I1)
        │     ├── Rubric Evaluation & Grade Matrix Service (I2, I3)
        │     └── Showcase & Fellowship Registry (I4)
        └── Distribution Services (Phase 3)
              ├── Publisher Imprint Portal & Rights Manager (P1, P5)
              ├── Steganographic ARC Watermark Engine (P2)
              ├── Sponsored Promotion Ad Server & Compliance (P3)
              └── Scouting & Manuscript Query Bridge (P5)
```

### 3.2 Data Storage Layer
* **Relational Database (PostgreSQL)**: Transactional data, user identities, cryptographic proofs, institutional grade transcripts, and publisher contracts.
* **Search Index (Elasticsearch)**: Sub-second search across book catalogs, reader essays, marginalia text, and authorial queries.
* **Cache (Redis)**: Live session marginalia streaming, read heatmaps, and taste-similarity cache.
* **Object Storage**: Manuscript revisions, book cover assets, cloth tokens, and watermarked PDF/EPUB proof files.
* **Event Stream (Kafka / Redis Streams)**: Real-time telemetry, reading dwell time, and reading club live marginalia synchronization.

---

## 4. Design System & UX Standards

* **Visual Identity**: Warm, bookish, tactile typography balancing editorial prestige and modern web ergonomics.
  * **Typography**: *Newsreader Roman* (display titles, manuscript prose, literary extracts) combined with *Plus Jakarta Sans* (interface controls, telemetry chips, data tables).
  * **Color Palette**: Forest pine (`#1b3b2b`, `#163323`), organic parchment cream (`#f7faf5`, `#faf2ed`), muted terra cotta, and warm amber accents.
* **Design Principles**:
  1. **Literary Dignity**: Minimize gamified streaks and star counts; celebrate long-form reflection and nuanced critique.
  2. **Authorial Consent**: Authors define their margin rights, reader inquiry anchors, and distribution exclusivity.
  3. **Algorithmic Transparency**: Promotions are explicitly tagged (`Sponsored`), and reviews are contextualized with reader taste concordance percentages.

---

## 5. Milestone & Release Roadmap

| Milestone | Deliverables | Status |
| :--- | :--- | :--- |
| **M1: Reader Core** | Feed (R1), Book Detail & Expectation Verdict (R2), Reader Match (R5), Shelf (R6), Reading Clubs (R8), Reader View (R9) | **Complete** |
| **M2: Writing & MFA Suite** | Drafting Suite (W1), Writers Guild (W4), Critique Desk (W4), Submission Modal (W3), Rubric Grading (I2/I3), Showcase (I4) | **Complete** |
| **M3: Publisher Suite** | Catalog Launch (P1), Steganographic ARC Pool (P2), Sponsored Ad Engine (P3), Scouting Desk (P5) | **Complete** |
| **M4: Interactive Protocol Bridges** | End-to-end W1 Drafting → P1/P2 Launch → R9 Reader Consumption Live Bridge | **Complete** |
