# Perch pre-development documentation pack

This pack contains draft product and architecture artefacts based on the Perch concept and Phase 1 reader use cases.

## Files

- `product/user-journey-maps.md` — four Phase 1 reader journeys and validation questions.
- `product/information-architecture.md` — Phase 1 sitemap, screen inventory and future-phase IA.
- `architecture/domain-model.md` — conceptual ER model, domain rules and future extensions.

## How to add these to your existing Git repository

Copy the `product/` and `architecture/` folders into your repository. A suggested location is:

```text
perch/
├── README.md
├── docs/
│   ├── product/
│   │   ├── prd.md
│   │   ├── user-journey-maps.md
│   │   └── information-architecture.md
│   └── architecture/
│       └── domain-model.md
└── ...
```

The PRD itself is a Markdown file. Copy the PRD content you have already drafted into `docs/product/prd.md`.

GitHub supports Mermaid diagrams in Markdown files, so the diagrams should render in the repository's file viewer.

These documents are drafts. Validate assumptions with reader research before treating them as final requirements or database design.
