Perch

A dedicated social space for books, built like Instagram. Readers discover books through other readers instead of through promotion feeds and marketplace reviews.
The idea
A book-first social platform: a feed of books and what readers think of them, in the format people already scroll.
Discovery through readers you trust, not through paid promotion or anonymous marketplace reviews.
Easy creation and publishing support for writers, so new voices reach readers directly.
A club for budding writers, with outreach to educational institutions for support and evaluation of aspiring writers.
Tie-ups with publishing houses for distribution. Not against Amazon; buying can still happen there.
Where it came from
Instagram promotions led to a few books that were not up to the mark. Checking Amazon and Google reviews did not prevent it. Reading Yellowface raised the question of how much PR shapes what reaches the shelf, and no existing product seemed to play this role.
Order of build
Readers first.
Writers next, once the reader base exists.
Publishing-house distribution after that.
End usersUserWho they areWhat they want from PerchReaderCame to books through social media. Reads around 15 physical books a year. Hears about books on Instagram, then friends, then bookstore bestseller tables. Buys on Amazon or in a bookstore.Find books they will actually like, before paying for them.Budding writerWriting something and wants readers and feedback.Create, publish, get evaluated, find an audience.Educational institutionTeaches or supports aspiring writers.A place to support and evaluate student writers.Publishing housePublishes and distributes books.Reach readers through a trusted channel.
Use case diagramflowchart LR
  Reader["Reader"]
  Writer["Budding writer"]
  Inst["Educational institution"]
  Pub["Publishing house"]

  subgraph Perch
    direction TB
    subgraph P1["Phase 1: readers"]
      UC1(["Browse a feed of books and reader posts"])
      UC2(["Check what readers think before buying"])
      UC3(["Post about a book"])
      UC4(["Follow readers with similar taste"])
      UC5(["Track books: want to read, reading, read"])
      UC6(["Buy through a link to Amazon or a bookstore"])
    end
    subgraph P2["Phase 2: writers"]
      UC7(["Create and publish writing"])
      UC8(["Get feedback and evaluation"])
      UC9(["Join a writers club"])
      UC10(["Support and evaluate aspiring writers"])
    end
    subgraph P3["Phase 3: distribution"]
      UC11(["Distribute books through Perch"])
    end
  end

  Reader --> UC1
  Reader --> UC2
  Reader --> UC3
  Reader --> UC4
  Reader --> UC5
  Reader --> UC6
  Reader -. reads .-> UC7
  Writer --> UC7
  Writer --> UC8
  Writer --> UC9
  Inst --> UC10
  Pub --> UC11
Use cases
Phase 1: readersIDUse caseActorUC1Browse a feed of books and reader postsReaderUC2Check what readers think of a book before buying itReaderUC3Post about a book: a reaction, a review, a recommendationReaderUC4Follow readers with similar tasteReaderUC5Track books as want to read, reading, or readReaderUC6Buy through a link to Amazon or a bookstoreReader
Phase 2: writersIDUse caseActorUC7Create and publish writing on the platformBudding writerUC8Get feedback and evaluation on published writingBudding writerUC9Join a writers clubBudding writerUC10Support and evaluate aspiring writersEducational institution
Phase 3: distributionIDUse caseActorUC11Distribute books to readers through PerchPublishing house
Reader use cases UC1, UC3, UC4, and UC5 are read off "like Instagram": feed, post, follow, save. Edit them if that is not what you meant.
