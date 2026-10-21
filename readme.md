# Interface Design Cards

Brainstorming-cards related to **Interface Design**.

- arrange & think & discuss!
- read between the cards!

[`interfacedesigncards.csongorb.com`](http://interfacedesigncards.csongorb.com)

## Structure

This repository holds **content only**. Everything that displays the cards comes from [cardsimulator](https://github.com/csongorb/cardsimulator), included as a git submodule (pinned to a commit).

- `cards/cardset.xml`: title, repository and public address (used by the QR codes in PDFs)
- `cards/cardCategories.xml`, `cards/cards.xml`: the cards
- `texts/`: documents linked from the cards
- `index.html`: tiny loader, identical in every card set
- `.github/workflows/deploy.yml`: publishes the site to GitHub Pages on every push to `main`
- `cardsimulator/`: the simulator (submodule)

Run locally with any static web server (the XML can't be loaded from `file://`): `python -m http.server`, then open http://localhost:8000/.

Update the simulator: `git -C cardsimulator pull origin main`, then commit the changed `cardsimulator` pointer.

## Version-History

### Release 1.1 (Work in Progress)

- some links updated
- repository is now content only (new card table from `cardsimulator`, `cards/cardset.xml`, GitHub Pages deploy workflow)
- category "games" renamed to "case studies"
- new color palette for the categories
- new case studies: Clair Obscur: Expedition 33, Outer Wilds
- book links point to the book's Wikipedia article (or its Goodreads page when there is none) instead of Amazon

### Release 1.0 (26. March 2021)

- first release
- created for Porn Creator 0.3
- primarily made to support a course at the UE
	- incl. all the links and topics I had already prepared for previous UI classes
