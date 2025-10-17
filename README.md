# Purpose
The goal of the TCG Data project is to provide a public data set concerning card and game details for dead collectible card games and trading card games to support software development, discussion, and interest regarding these games.

# Scope
This project is focused on documenting dead TCGs.  

A game is considered a "TCG" for this project if players are expected to assemble their own beginning game items out of their own collections before beginning a game.  "Deck Building" games such as Dominion, or Ascension that include all components for all players and expect the players to assemble their decks out of this shared pool during the course of the game are out of scope for this project. "LCGs" like Doomtown: Reloaded or Android: Netrunner that are sold as full sets, but still require expect players to assemble their own sets of beginning components are in scope for this project.

A game does not need to be limited to cards, such as Dice Masters, nor does it need to use cards at all, such as Dragon Dice, to be in scope for this project. 

A TCG is considered "dead" when it has been cancelled by it's designers and is not expected to receive new additions.  We may choose to include a game that is later revived, such as Overpower, but we will not cover the new publisher's additions.  This chose is primarily due to the additional resources needed to provide ongoing coverage to a "live" game.

# Sources
Any item data used in the TCG Data project must be from an appropriate source.

The ranking of sources from most preferred to least preferred is
* A physical copy of an actual game item in the possession of a trusted TCG Data Project contributor
* A photograph of a physical game item
* An official document from the publisher of the game
* A document from a trusted third party source

# Definitions of Done
Item Complete: A Game or Set is labeled as Item Complete when we believe we have an entry for every item in that game or set in our dataset.
Data Complete: A Game or Set is labeled as Data Complete when we have included all attribute data for each item in that game or set in our dataset.
Image Complete: A Game or Set is labeled as Image Complete when we have created, or been donated high quality images covering all relevant attributes of each item in the game or set.

# Style Guide
Our goal is to accurately document TCGs as they were designed and released. Whereever possible, the style and errors present in a release item should be preserved.  If their is a need to include corrections or errata, they should be included in addition to the original, published form. 

# Data
All items in the dataset shall have at least the following values

- tcgdata_item_id - a unique id across all items from all games
- name - a string naming the item.  This item should represent a functionally unique game item.  Different items in the same game line with the exact same game function may share the same name value, but should have disambigution attributes in the attributes value. 
- game - a string identifying the game this object is from.  All values in this field should be unique to the game they represent.
- set - a string identifying a set of cards this object is from.  This value may be null.
- source - a string indicating the source of the data for this item.   Acceptable values are ("item", "photo", "first-party-document", "third-party-document")
- images - a JSON list of filenames without extensions that can be used to uniquely identify images for the item.
- attributes - a JSON object describing all relevant attributes of the game item.

# Supported Data Formats
Currently, we intend to maintain per-game CSVs with all item data. These CSVs will be regenerated as needed from our project database.  We also intend to move our database files into github when we are able.

Our desire is to provide a robust set of data formats to support other projects.  If you have a project that would benefit from different data formats, please reach out or create an issue. 

# Current Game Statuses
## Rage - Item Complete - Images: 1099/1294 (85%)
- Limited Edition - Data Complete - Images: 307/321 (96%)
- Unlimited Edition - Data Complete - Images: 319/321 (99%)
- The Umbra - Data Complete - Image Complete: 95/95 (100%)
- The Wyrm - Data Complete - Images: 143/185 (77%)
- The War of the Amazon - Item Complete - Images: 75/140 (54%)
- Legacy of the Tribes - Item Complete - Images: 159/215 (74%)

https://archive.org/details/rage-ccg_hd-scans

## The Crow - Data Complete: 123/123 - Images: 26/123 (21%)
- Limited Edition - Data Complete 122/122 - Images: 26/122 (21%)
- Promo - Data Complete 1/1 - Images: 0/1 (0%)

https://archive.org/details/the-crow_card-scans

