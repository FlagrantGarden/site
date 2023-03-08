---
author: Mikey Lombardi
date: 2022-07-28
title: The WOP Model
linktitle: The 🤌🏻 WOP 🤌🏻 Model
summary: |
  Thoughts on the Web, Offline, Physical (WOP) model of tabletop text production
categories:
  - meta
tags:
  - workflow
  - production
weight: 10
type: posts
---

There's endless ways to work on games-adjacent texts and projects. This one is mine.

I've been adopting the WOP model for releasing projects. In the WOP model, independent publishers
choose to release three broad editions of our works: Web, Offline, and Physical, in roughly that
order.

The rest of this post will set some context then elaborate on each edition in turn.

## Context

There are a few things I think are true about games-adjacent texts when it comes to independent
production[^1].

1. Everyone has a limited budget.
1. Everyone has limited time.
1. Everyone has limited skills.
1. Everyone has differing accessibility needs.
1. Everyone has differing aesthetic preferences.
1. Digital formats aren't physical formats.
1. Reference texts aren't teaching texts.
1. Production can be iterative rather than incremental.

I'm not going to belabor the first five points. If you aren't limited by budget, time, or skill,
good for you. If you think that accessibility is one-size-fits-all, you're wrong and I encourage
you to use a search engine. If you think everyone shares the same aesthetic preferences, I encourage
you to talk to more people.

### Digital Formats Aren't Physical Formats

This is trivially true but I want to hammer this point home and expand on it. I see a lot of people
not getting it and when I _do_ mention it there's usually Discussion.

When you make a PDF for printing, you're almost certainly prioritizing a _relatively_ flat and
non-interactive document. You can make fantastic books and incorporate all sorts of interactivity
into them but, to be clear: that's not largely what people are doing. They're making functional
books with some attention paid to layout and interspersed with as much art as they can afford. Which
is fine!

But then they turn around and release those PDFs as the "digital" edition of their work and _almost
always_ without further updating the PDF. So the PDF is usually:

- in portrait orientation
- with text sized as appropriate to the print format
- without alt text or tagging
- without updated metadata
- without the language set
- without cross-reference linking

The PDF is also often without:

- a TOC
- bookmarks
- the text ordered in a way screen readers can sensibly parse

Print formats are limited by their medium. For most games-adjacent texts, this means "ink on
nearly identical physical pages, organized into spreads."

Digital formats are limited by their specific implementation (EPUBs are somewhat more limited than
web pages).

A non-exhaustive list of things you can do in a digital format that you can't do in the physical
formats[^2]:

- have flexible display settings, like:
  - changing the size, color, and spacing of text and other elements
  - automatically adjusting layout based on the viewer's context (viewport size, light/dark theme
    preferences, etc)
  - switching to a different font (e.g. to a more readable font for folks with dyslexia)
- embed additional media like audio and video
- update your work nearly on-demand

Web formats add even more functionality:

- interactive elements generally, such as:
  - clickable buttons to do something like generate a prompt, show a random item, or roll on
    a table
  - expandable/hidable content
  - filtering/sorting tables and lists
  - integrations with other services, like discord or RSS feeds
  - modals (pop-over content) to do things like export characters or adventure ideas
  - widgets to present information in a transformable/inspectable way
- downloadable content
- cross reference _between_ texts

### Reference Texts Aren't Teaching Texts

My day job is technical writing. People in games often talk about technical writing. Most of the
people talking don't appear to have a technical writing background.

I've [talked before][3f-talk] about a [threefold model][3f-site] of documentation which breaks down
into conceptual, narrative, and reference documents. Of those three, narrative documents are _most
frequently_ teaching texts. They have a specific set of learning goals for a specific audience. Some
conceptual documents are also teaching texts, covering a particular domain (or subdomain) in detail.

An even better model is [Daniele Procida][Procida]'s four-kinds taxonomy, which distinguishes
between learning-oriented tutorials, goal-oriented how-to guides, understanding-oriented
discussions, and information-oriented reference material.

Notice that under neither model are reference texts the same thing as teaching texts. Referencing
and learning are different activities. The structure and content of your text should be specific
to its purpose.

### Iterative and Incremental Production

I came up in tech where the question of whether to work incrementally or iteratively is _pretty well
settled_. Incremental production is when you go step-by-step through your process doing one piece as
fully to completion as you can before moving onto the next. Iterative production is continuously
making small changes and improvements to your work.

Compare the following approaches:

1. You're working on a book without illustrations. You write an outline and rework it until you're
   satisfied. Then you write each chapter in the order they're placed in the outline in your layout
   software, tweaking the presentation as you go. When you're pretty sure you're done, you bring in
   an editor take a pass on the text and, when you're happy with things, you send it to print and
   call it done.
1. You're working on a book without illustrations. You write a draft of your outline then start
   writing your book, editing and reworking your outline and each chapter as you go. You have your
   developmental editor take a pass on each chapter as soon as you think that section is done. When
   your text is complete, your editor starts a copy editing pass. Once you're text-complete, you
   move onto layout, doing a rough blocking for the project, copying your text in without styling it
   extensively. Next you do a broad styling pass to see how things look and if you need to add
   references, appendices, or other changes. Then you standardize everything and finally go through
   and verify everything before your editor takes a final line edit pass. Sure that you've made no
   mistakes, you send it to print and call it done.

The first approach is broadly incremental, the second iterative. All projects tend to be some
combination of iterative and incremental---there are some tasks blocked by others and everyone goes
back to update things at some point---but projects _tend_ to be more one or the other.

The advantage of iterative development for a solo developer is noticeable but not particularly
groundbreaking. The most visible difference is how quickly and smoothly you can adapt to changes or
mistakes. An iterative approach tends to be more flexible and in many fields the [data][dora] shows
that it helps reduce mistakes, speed up releases, and makes for safer work environments.

For games-adjacent work, the flexibility and impacts on getting our work published are probably the
advantages independent publishers will notice the most. The other benefits aren't _nothing_,
especially for larger teams.
especially for larger teams.

## Web

The web edition is critically useful for a few reasons.

1. The tools you need to make them are free or cheap and bounded more by your time and energy than
   anything else. You can make a website in under an hour with free tools or continuously improve
   your own website on a custom domain.
1. They can be as minimal or extravagantly detailed as you please.
1. They can be iteratively written, shared, improved, and reworked without substantial costs.
1. They're functionally advertising, even if you don't invest in that. Merely existing online gives
   people a chance to stumble on your work from a search engine. If you already have content on your
   site, every update, release, or blog post is another chance for people to see your work.
1. You're not stuck trying to cram everything into a single flow of pages. While you're still
   developing the text, you can reorder things, add reference pages, try writing focused teaching
   texts, add supporting media, post experimental ideas as blogs, and more.

As I noted [above](#digital-formats-arent-physical-formats), web editions are also a richer and more
accessible option than PDFs.

Focusing first on releasing a web edition gives me flexibility, accessibility, interactivity, and
visibility that I would have to work much harder to get with a PDF-first model, if I could get those
benefits at all.

When I talk about making web editions, I always hear three main lines of concern.

<!-- vale Microsoft.HeadingPunctuation = NO -->

### How will I get people to buy my thing if they can find it online for free?

Lucky for you, it's possible to gate your web content behind a paywall if you _really_ want
to. I actually advise folks not to do this though for several reasons:

- Your web edition _is also advertising_ for your offline/physical editions and other works.
- A web edition is a phenomenal "try before you buy" option. If your web edition is done well,
people are likely to want a physical copy. It's constantly remarked on in developer circles that
  our audiences love to buy cool shit.
- People also often complain about piracy. Producing a low-to-no-art highly interactive and
  accessible version of your work as part of your general development cycle _and letting people
  find it and play with it_ is certainly not _worse_ than piracy.
- Is the goal of your project to get people playing with the thing you made, to make money, to
  express yourself, or a combination? I haven't seen _any_ evidence to suggest that a good web
  edition of a project negatively impacts sales and several times people have talked about how
  their Carrd site or free quickstart rules or whatever _helped_ make sales.

### I don't have the skills to make a website, isn't it hard?

It definitely _does_ take skill and effort but _so does making a nice PDF or print book_. If you
don't want to learn the skills or spend the time you can _always_ use tools like Carrd or a
specialized editor that helps you put things together.

You can hire someone to do it for you. Lots of people (like me!) already do that for print
layout. And, like everything around independent production, if you don't have the cash-on-hand to
hire someone as a contractor there's tons of other options. One of the better options you have is
to _bring someone with the skills into your core team_ and collaboratively run things as a
cooperative.

You can also learn. There's an unbelievable amount of resources on web development including
videos, training courses, books, blogs, and a huge number of people amongst your peers who have
the skills and are happy to teach your or help.

I've also been working on [tools][platen] and [workflows][blog-wf] to make web editions for books
easier. My goal with these projects is to make it merely as much work to make a great web edition
for your project as a physical edition.

### Don't you need reliable internet and a good computer to use a fancy website?

Strictly speaking, you don't need to be online to access websites anymore. A lot of static sites
and site hosts support [Progressive Web Apps (PWAs)][pwa] which let users hit the site once and
then access it (and most of its functionality) later, even if they don't have an internet
connection. Even better, PWAs can be treated like apps on mobile devices, making your work easier
to find once someone has decided they like it enough to pin it. Yes, you need to have internet
access at least once but that's _also_ true for PDFs.

If a website is made correctly, you _don't_ need a powerful computer to access and enjoy browsing
it. Especially for the types of content and interactivity we're highlighting for books, there's
_nothing_ you need to put in a web edition that should require more than 3g connectivity and a
Chromebook, phone, or tablet.

<!-- vale Microsoft.HeadingPunctuation = YES -->

## Offline

People also like reading texts on e-reader screens or printing them off at home to share with
their friends. Sometimes people just find that parsing printed text is less work for their brains.

So in addition to a web edition, I also propose and endorse creating an offline edition of your
work. For me, this actually comes in two related forms: an EPUB and a print-at-home PDF option.

### EPUB

I advocate without reservation that everyone make an EPUB for every text they're releasing in any
sort of digital format. If you're not into a web edition or a print-at-home offline option, make an
EPUB anyway. EPUBs are _widely_ supported---you can read them on any phone or tablet, in nearly any
computer browser (with an add-on) and on any computer (with an app), and on e-readers.

If you're making a web edition, chances are _very good_ you're writing in Markdown and using a
static site generator which means you _already have what you need to make an EPUB_. You can use
software like [Pandoc][pandoc] or [online tools][epub-online] to convert your Markdown to an EPUB.
Unless something has gone horribly wrong, all you need to do at that point is add metadata and make
your EPUB available.

### Print-at-Home

In addition to making an EPUB, I suggest making a PDF with low ink usage and a layout focused on
readability that's meant to be printed on a home printer (or at a local print service, often
co-located with shipping---check your local area).

I've personally been leaning towards letter/A4 sized PDFs you can print double-sided, three-hole
punch, and shove in a binder. You could also do a zine or pocketmod format, whatever works for your
project.

Where the web edition focused on interactivity and taking advantage of being read on a screen, a
print-at-home edition of your work should focus on being as usable and helpful as possible once it's
printed. This is where I suggest you start spending money and/or time on illustrations, assets, and
supporting materials.

An offline edition for printing at home could include:

- paper minis - who doesn't love nasty little freaks you can print, cut, and color?
- paper terrain - print and fold for suddenly three-dimensional play spaces
- tokens - spell or condition effects, interactive or destructible items, trackers
- maps - small, large format, illustrative
- tiles - hexes, buildings in a town, a boat, dungeon sections
- quick reference sheets - rules, spells, factions, rumors, regions
- cards - to print on cardstock and cut, print directly onto index cards, or print on paper and glue
  to index cards
- pregenerated characters - combine quick reference, quick start, and an idea to get people going
- handouts - letters, portraits, scene illustrations, spell books, ledgers, job boards

You're not limited to what you can afford to have professionally printed, packed, and shipped but by
your own imagination and tolerance for work (or budget/team if, like me, you're incompetent at both
layout and illustration).

You also don't have to have everything solved or ready all at once. Unlike a physical edition, which
people buy and expect to show up intact, packed, and ready to go, your offline edition can always
add more stuff and fix issues. Like your web edition, you can iterate as much as you please with
very little overhead.

### LeanPub

When it comes to selling offline editions of your work, I recommend [LeanPub][leanpub]. LeanPub has
a [category for Roleplaying Games][leanpub-rpgs] and you won't need to buy a subscription (none of
those features matter if you're making your own EPUB/PDF). LeanPub _does_ take 20% of sales
revenue---more than Itch, less than DTRPG---but LeanPub also:

- pays royalties promptly and reliably
- has a functional search/discovery experience
- has excellent and responsive support
- highlights projects regularly
- supports and encourages you to sell your work elsewhere
- has an audience that _expects_ work to arrive in an unfinished state and improve over time
- has functional feedback and following mechanisms for readers
- lets readers opt-in to sharing their email with you, which you can integrate directly with
  Mailchimp if you want
- lets you notify readers when you've updated your book, if you want (separate from mailing list)
- allows you to split your revenue amongst your collaborators automatically---you don't need to hold
  cash and do payouts, LeanPub will handle that for you
- enables you to automatically direct some or all your revenue to a charitable organization
- has a functional newsletter you can spend revenue to secure a spot in (they also highlight
  projects that _don't_ spend money)
- lets you sell multiple packages of your project at varying prices (e.g. just the text, text +
  assets, text + assets + consulting/custom content)
- enables you to set a minimum price and a suggested price and uses a price slider that _starts_ at
  the suggested price (my experience is that many people actually pay _more_ than the suggested
  price)
- supports coupons (which you can use to mimic community copies, if you want)
- has robust settings including:
  - a community edition (free copy with optionally limited content that people get in exchange for
    opting to provide their email address)
  - a sample edition (free copy with optionally limited content, no conditions)
  - the ability to temporarily unlist your book
  - provide your book in multiple languages
  - incorporate team bios
  - set a thank you message for purchases

For me, the most useful features are the automatic revenue sharing with the team and being able to
direct revenue to a charity organization. I find that this is worth the 20% cut even before
considering the rest of the features and benefits.

When it comes to pricing, I'm comfortable selling my work on LeanPub at similar rates to those
people are charging for physical copies. I set the suggested price where I think it ought to be and
then fiddle with my minimum price (usually in the $8--12 range). One model I really like on LeanPub
is to start the price lower when I first release and increase it as my team adds assets and improves
the core text. For example, I might put a book up with a $8/$16 minimum/suggested price and raise
them $1/$2 every month that we add stuff until the price is $16/$32.

Remember, you can have add-ons packages and price those separately.

## Physical

I approach physical editions a little differently. I may not do a physical edition for every
project---it depends on how much interest and excitement there is in both the team and the audience.
When I do, I aim for a luxury option. Because I release a free web edition and an affordable offline
edition, I don't worry about how affordable or limited my physical editions may be. Instead I can
work with the team to manifest the best possible expression of our work in physical form.

In practical terms, this means making exactly the physical edition we want with the printing,
layout, assets, and every possible option we think is best. We work out what we want to do together,
propose ideas, figure out the budget and the long term plan, then execute.

This means we can more comfortably do things like limited run box sets, high quality books, and
weird experimental projects that may not see a reprint. We can lean all the way in on "will this be
cool/fun/awesome in someone's hands?" and not feel like there's any need to compromise because we're
only really getting one edition to work with. If we didn't have the web or offline editions, this
would be much harder to justify.

For example, the rough plans right now for the physical edition of _Flagrant Factions_ (web edition
nearly text-complete) include:

- Printing 216 copies of the text on dyed mulberry paper (probably risograph printing, _possibly_
  screen printing if my experiment works out and I don't want to eat dynamite after doing a couple
  test prints) numbered 111.111--111.666 (the next print run, if any, would be 112.111--112.666),
  loose-leaf and three hole punched. The combination of ink and paper used in the print run will
  never be repeated.
- Putting the copies in custom mulberry paper envelopes with a wax seal.
- Setting aside copies 111--166 to be sold with their own custom hand-made binders and slip cases
- Having a sort of "made to order" option where buyers of 111--166 can choose to add on a chest
  which replaces the slipcase and holds:
  - cut-and burned versions of the tokens and paper minis
  - wooden interlocking tiles for each of the locations
  - dice, pencils, tape measure, etc
  - probably more bullshit I haven't dreamed up yet or forgot and will remember eventually

Whereas the rough plans for the physical edition of _A Treatise Chymic_ (currently in early draft)
include:

- A coptic-bound book with bronze plates containing the text
- A chymist's book of formulae, including quick references so it's all you need to play a chymist at
  the table, each with random starting formulae already added and some notes/quests for discovering
  more of them
- A chymist's notebook of ingredients with the well-known ingredients already documented and space
  to describe, annotate, and illustrate new ones
- A "So You Want to be a Chymist?" pamphlet with streamlined information for adapting chymistry to
  specific systems
- Handouts for the various quests and NPCs described in the core book

When I talk about being able to _really_ lean in on our wild ideas for physical, this is where I'm
headed. That doesn't mean you should (or even that these are good ideas!) but I think this is only
really enabled _because_ my model includes web and offline editions. If I was doing things the
traditional way, I'd just have a PDF that was meant to be everything all at once and have to
compromise endlessly to get something passable.

I choose to go another way. Maybe you will too.

<!-- vale alex.Condescending = NO -->

[^1]: I'm using the term "production" here because I mean to talk about more than _just_ writing.

[^2]: You can do things in physical you can't easily do in digital, like hold several pages open at
once and flip rapidly back and forth between them. There's also a lot you can do with physical books
if you're playing around more with form and format, but nearly no one is.

[3f-talk]:      https://www.youtube.com/watch?v=0S0eAuGzjpI&t=2s
[3f-site]:      http://michaeltlombardi.gitlab.io/needful-docs/
[Procida]:      https://www.writethedocs.org/videos/eu/2017/the-four-kinds-of-documentation-and-why-you-need-to-understand-what-they-are-daniele-procida/
[dora]:         https://services.google.com/fh/files/misc/state-of-devops-2021.pdf
[pwa]:          https://web.dev/progressive-web-apps/
[platen]:       https://github.com/platenio/platen-template
[blog-wf]:      https://flagrant.garden/posts/writing-markdown/
[pandoc]:       https://pandoc.org/
[epub-online]:  https://www.google.com/search?q=markdown+to+epub+online
[leanpub]:      https://leanpub.com/
[leanpub-rpgs]: https://leanpub.com/bookstore?category=roleplaying_games&type=all
