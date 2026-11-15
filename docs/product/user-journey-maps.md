# Perch — Phase 1 User Journey Maps

**Platform:** Desktop-first responsive web application.

## Journey 1: New Reader Onboarding and First Discovery

**Goal:** Help a new reader discover relevant books and reader perspectives without requiring them to follow anyone first.

| Stage | User action | Potential friction | Product opportunity |
|---|---|---|---|
| Landing | Opens Perch in a browser | Doesn't understand the value proposition | Explain reader-led discovery with a sample feed |
| Sign up | Creates an account | Long registration process | Keep registration minimal |
| Taste setup | Selects genres, favourite books or preferences | Too many questions | Make preference setup short and skippable |
| First feed | Views the Home feed | Empty or irrelevant content | Seed discovery using selected interests |
| Explore | Opens a book or reader post | Doesn't understand why it was recommended | Show reader context and recommendation source |
| Return | Saves a book or follows a reader | Actions are difficult to locate | Make save and follow actions visible |

**Web experience considerations**
- Landing page should communicate Perch's purpose immediately.
- On desktop, use persistent left navigation and a central feed.
- An optional right sidebar can display suggested readers or genres.
- The feed must be useful even when the user follows nobody.

**Success signals**
- Sign-up completion.
- First book-detail visit.
- First shelf addition.
- First reader follow.

**Research questions**
- What makes a reader trust a recommendation?
- Which onboarding preferences are useful?
- Does a sample feed communicate the product's value?
- What is the most natural first action?

---

## Journey 2: Evaluate a Book Before Buying

**Goal:** Help a reader decide whether a book is worth buying through opinions from other readers.

| Stage | User action | Potential friction | Product opportunity |
|---|---|---|---|
| Discover | Finds a book through the feed or search | Doesn't know why the book appeared | Show who shared it |
| Open detail | Visits the book page | Generic metadata dominates | Prioritise reader opinions |
| Compare opinions | Reads reviews and ratings | Enjoyment and expectation match are confused | Keep these ratings separate |
| Check taste relevance | Looks at opinions from similar readers | Similarity feels arbitrary | Explain why readers are considered similar |
| Decide | Saves the book or opens a retailer link | External purchase destination is unclear | Clearly label external purchase links |

**Web experience considerations**
- Use a dedicated, shareable book-detail page.
- Display book information and shelf actions prominently.
- Prioritise reader reviews over generic promotional descriptions.
- Keep enjoyment and expectation-match ratings visually distinct.
- Clearly identify links that take users to external retailers.

**Success signals**
- Book-detail engagement.
- Review interactions.
- Shelf additions.
- External purchase clicks.

**Research questions**
- Which reader signals influence purchase decisions?
- Do users understand the difference between enjoyment and expectation match?
- What makes a taste match credible?
- How many reviews are needed before a book page feels useful?

---

## Journey 3: Publish a Book Post or Review

**Goal:** Allow readers to share opinions that help other readers make better discovery decisions.

| Stage | User action | Potential friction | Product opportunity |
|---|---|---|---|
| Start | Selects Create from the sidebar | Unclear difference between a post and review | Offer clear post types or a unified composer |
| Attach book | Searches for a book | Duplicate or incomplete book metadata | Provide a searchable book picker |
| Write | Adds a reaction or review | Writing feels like a form-filling exercise | Keep free text central and prompts optional |
| Rate | Adds ratings | Rating concepts are confusing | Explain enjoyment and expectation match separately |
| Preview | Reviews the post | Formatting or visibility surprises | Provide a preview and spoiler controls |
| Publish | Publishes the post | No confirmation or next step | Show confirmation and published-post link |
| Engage | Responds to comments | Notification overload | Provide useful notification preferences |

**Web experience considerations**
- Prefer a dedicated compose page for longer reviews.
- Consider a two-column editor and preview layout on desktop.
- Provide draft-saving feedback.
- Make spoiler and visibility controls explicit.
- Keep the composer focused and uncluttered.

**Success signals**
- Composer starts.
- Draft completion.
- Publish completion.
- Meaningful comments and interactions.

**Research questions**
- Do readers distinguish reactions from reviews?
- Which fields should be optional?
- Is a live preview useful?
- What spoiler controls do readers expect?

---

## Journey 4: Build a Trusted Reader Network

**Goal:** Help readers discover and follow people whose opinions and reading preferences they find valuable.

| Stage | User action | Potential friction | Product opportunity |
|---|---|---|---|
| Notice reader | Sees a reader on a post | Reader identity is too limited | Provide a profile preview |
| Visit profile | Opens the reader's profile | Profile focuses on follower counts | Highlight shelves, reviews and genres |
| Assess fit | Browses reading history | Similarity claims lack evidence | Show shared books and genre overlap |
| Follow | Selects Follow | Follow state is unclear | Provide immediate visual feedback |
| Return | Goes back to Home | Followed content isn't reflected | Incorporate followed-reader posts into the feed |

**Web experience considerations**
- Profiles should have shareable URLs.
- Use clear sections for Posts/Reviews, Shelves and Activity.
- Keep follow actions visible.
- Do not make follower count the primary measure of trust.

**Success signals**
- Profile visits.
- Follow conversions.
- Engagement with followed-reader posts.
- Repeat visits.

**Research questions**
- What makes a reader worth following?
- Are shared books or shared genres stronger taste indicators?
- Which profile sections are most useful?
- How should Perch explain similarity without suggesting certainty?

---

## Cross-Journey Principles

1. The feed must provide value before a user follows anyone.
2. Reader context should appear wherever a recommendation appears.
3. Enjoyment and expectation match are separate concepts.
4. Taste similarity should be explainable and appropriately qualified.
5. External purchase links must be clearly identified.
6. Useful discovery and trust matter more than vanity engagement.
7. Core journeys should support keyboard navigation and accessible focus states.
