# KinDex - Your Family as Collectible Cards

KinDex turns your family tree into a deck of collectible trading cards. Every relative gets a card with their photo, their family links and their story, and the whole family is laid out as a tree you can explore.

The name comes from **Kin** + **Index**: a card index of your kin, the people in your family.

- **Private by design.** Everything happens in your browser. Your family tree and photos are never uploaded anywhere.
- **Nothing to install.** KinDex is a single web page that works in any modern browser, on a computer or a phone.
- **Works with your family tree app.** It reads the standard GEDCOM file that almost all of them can export.

## Why KinDex?

A family tree is full of names and dates that are easy to scroll past, especially for children. KinDex was made to get young ones curious about their roots, so every ancestor becomes a card worth collecting.

As collectible cards, the people who came before become characters to discover. Children can flip through the deck, see what each relative did and where they lived, follow the links from card to card, and find out who the rarest cards in the family are: the ones furthest back in the tree.

## Try it

Want to see it first? Click **▶ Try a sample family** on the home page to explore the Hartwell family: a fictional family of 20 people over 6 generations.

## What is GEDCOM?

GEDCOM (`.ged`) is the standard file format family tree apps use to save and exchange trees. It holds names, dates, places, relationships and notes, so you can move a tree from one app to another.

You can export one from Family Echo, Ancestry, MyHeritage, FamilySearch, Gramps, RootsMagic, Legacy, PAF and most other family tree apps. Look for an option like **Export**, **Download** or **Share** and choose **GEDCOM**. In Family Echo, for example, it's *Share → Export → GEDCOM*.

KinDex reads GEDCOM versions 5.5, 5.5.1 and 7.0.

A GEDCOM file doesn't contain the photos themselves. That's why KinDex lets you add them from a folder (see below).

## Getting started

### 1. Export your tree

Export your family tree as a `.ged` file from your family tree app.

### 2. Add photos (optional)

Make a folder for your family. Put the `.ged` file in it, and add a `photos` folder with one photo per person, **named after that person**:

```
Hartwell Family/
├── hartwell-family.ged
└── photos/
    ├── Arthur Hartwell.jpg
    ├── Thomas Hartwell.png
    └── Daniel Kim.jpg
```

- Capitals, spaces, hyphens, underscores and accents don't matter: `daniel-kim.png` and `DANIEL_KIM.jpg` both match Daniel Kim.
- If two people share a name, add the birth year: `Maya Hartwell 1983.jpg`.
- People without a photo get a card with their initials.

### 3. Open it in KinDex

- **Open family folder** opens the whole folder: the tree and all the photos.
- **Open a .ged file** opens just the tree. You can select photos at the same time.
- Or **drag and drop** the folder, a `.ged` file or photos onto the page.

Your browser may ask whether to let the site **view files**. That only lets the page read them on your device; nothing is sent anywhere.

To update your cards later, export the tree again over the old `.ged` file or add more photos, then click **↻ Reload**.

## What you'll see

Everything on a card comes from your GEDCOM file and your photos: names, dates, places, relationships, notes and pictures. KinDex doesn't add, change or check any details about your family. It only shows what your file already contains, in the style of a collectible card. If something on a card is missing or wrong, fix it in your family tree app and export the file again.

The game-style parts of a card, its rarity, type and card number, are just for fun. KinDex works them out from the tree itself.

### The family tree

Every person appears as a card, arranged by generation, with the oldest at the top. A gold line joins a couple, and a dashed line marks a former partner.

- Drag to move around, and use the mouse wheel, a pinch or the **−** / **+** buttons to zoom. **Fit** shows the whole tree.
- **Find a person** jumps straight to anyone's card.
- **Collection** shows all the cards grouped by generation, like pages in a binder.

### A card

Click any card to open it.

**The front** shows:
- the person's name, generation and photo
- a short summary: family name, gender, and their birth and age or the years they lived
- their family links: parents, partner and children
- how many siblings, children and descendants they have
- a quote from their notes, or their occupation and birthplace when there are no notes

**The back** is their *Family Record*: full name, nickname, dates and places of birth, death and burial, occupation, education, parents, partners and marriages, children, siblings and their complete notes.

- Click a relative's name to jump to their card.
- Click anywhere else on the card, or **↻ Flip**, to turn it over.
- Use the arrow keys for the previous or next card, `F` to flip, `S` to save an image, `T` to show the person in the tree and `Esc` to close. Press `?` or the keyboard button to see every shortcut.
- **⬇ Save image** saves the side you're looking at as a picture.
- **⌖ Show in tree** takes you to that person in the family tree.

### How cards are ranked

Each generation has its own rarity, from the oldest generation down:

| Rarity | Generation | Card border |
|---|---|---|
| ♛ Origin | 1st, where the tree begins | Black and gold |
| ★★★ Legendary | 2nd | Rainbow |
| ★★ Epic | 3rd | Purple |
| ★ Rare | 4th | Gold |
| ◆ Uncommon | 5th | Silver |
| ● Common | 6th | Sand |

In trees with more than 6 generations, neighbouring generations share a rarity.

- **Type:** each family name gets one of ten elemental types (Fire, Water, Grass, Lightning and others), which sets the colours of its cards.
- **In Memoriam:** relatives who have passed away get a 🕊️ badge and a thin silver ring around their card.

## Sharing with family

**Download to share** saves your whole family, with every card and photo, as one file. Send it to relatives by email, chat or a shared drive. They just open it in their browser: no folder, no app and no setup.

- The file contains your whole tree, including notes, dates and places. **Share it only with family.**
- When your tree changes, download a new file and send that instead.
- To share a single card, open it and use **⬇ Save image**.

On a phone, open the shared file in a browser such as Chrome or Safari. Some phone file previews (iPhone's Files preview, for example) don't run it.

## Privacy

- **Nothing is uploaded.** Your tree and photos are read and turned into cards inside your browser.
- **Nothing is kept.** Close the page and it forgets your tree. Nothing is stored, collected or shared.
- **Downloads stay with you.** Saved images and shared files are made on your device.

## Good to know

- **GEDZIP files** (`.gdz`, a zip with photos inside) can't be opened directly yet. Unzip it and open the folder.
- **Save image** works in Chrome, Edge and Firefox. Safari may not allow it, and KinDex tells you if so.
- **Very large trees** can have some crossing lines between families joined by marriage.

## What KinDex reads from a GEDCOM file

KinDex only needs standard GEDCOM. It also understands a few extras that some apps add.

| Area | What is read |
|---|---|
| Text | UTF-8, UTF-16, Windows-1252 ("ANSI") and ANSEL, detected automatically |
| People | Birth name (preferred over married names), nickname, gender, occupation, education and notes |
| Life events | Birth, or baptism if there is no birth date; death, or burial or cremation if there is no death date |
| Dates | Exact and approximate dates (`ABT`, `BEF`, `BET … AND`), dual years (`1750/51`), BC dates and other calendars |
| Families | Partners, marriages, divorces and children. Earlier partners of someone who remarried show as former partners. |
| Parents | Birth parents first; adoptive or foster parents also appear on the card back |
| Photos | Photos linked in the file, plus photos from your family folder |

Anything KinDex doesn't use is ignored, so a file never fails to open because of it.

## License

KinDex is released under the [MIT License](LICENSE).
