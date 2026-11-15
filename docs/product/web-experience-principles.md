# Perch — Web Experience Principles

## 1. Platform Decision

Perch is a **desktop-first responsive web application**.

Desktop and laptop browsers are the primary design targets. Tablet and mobile browsers should remain usable, but this is not a native mobile application specification.

## 2. Layout Principles

1. **Persistent navigation:** Keep primary navigation visible on desktop.
2. **Content-first reading:** Give book reviews and reader perspectives comfortable reading width and whitespace.
3. **Progressive density:** Use a main content column with an optional contextual right sidebar on wide screens.
4. **Stable destinations:** Book pages, reader profiles and posts should have shareable URLs.
5. **Clear information hierarchy:** Distinguish book metadata, reader opinions, enjoyment ratings and expectation-match ratings.
6. **Visible interaction state:** Follow, shelf, reaction and save states should be visible without hover.
7. **Accessibility:** Support keyboard navigation, visible focus, semantic structure, sufficient contrast and labelled controls.

## 3. Interaction Patterns

- Prefer full pages for tasks requiring context or longer reading.
- Use modals for short, focused actions only.
- Preserve drafts where feasible and communicate save status.
- Introduce filters and sorting sparingly in the first release.
- Clearly identify outbound purchase links as external destinations.
- Provide clear loading, empty, error and confirmation states.

## 4. Responsive Behaviour

| Viewport | Expected behaviour |
|---|---|
| Wide desktop | Persistent sidebar, main content and optional right sidebar |
| Small desktop | Narrow or collapsible sidebar; hide right sidebar first |
| Tablet | Compact navigation and single-column content |
| Mobile browser | Compact navigation and single-column layout |

The same information architecture should work across viewport sizes. Separate mobile-only product flows are not required unless research identifies a need.

## 5. Quality Expectations

- Prioritise fast initial rendering of the feed and book pages.
- Load lower-priority media progressively.
- Avoid layout shifts as book covers and avatars load.
- Ensure browser refresh and deep links work on core pages.
- Make empty, loading, error and offline states understandable.

## 6. Out of Scope

This document does not prescribe:
- Frontend framework.
- CSS framework or component library.
- Backend architecture.
- Database technology.
- Hosting provider.
- Native mobile application implementation.

These are separate technical decisions.
