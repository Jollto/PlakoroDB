# Plakoro (Fan Translation)

An unofficial database and fan translation for the Pokémon's dice game **Plakoro**.

> [!IMPORTANT]
> This project is **unofficial** and is **not affiliated with, endorsed by, or sponsored by the original developers or publisher.**

## About

This repository aims to provide translations of Plakoro cards for players who cannot read Japanese.

The translations are created by fans and are intended to be as accurate and consistent as possible, following official terminology whenever it exists and the writing conventions commonly used in trading card games.

Some moves might not have an official translation in either the TCG game or on the videogames. Attack names that are still uncertain are marked with a **?** in the text files and may change in the future if an official translation is released.

The translations are being made in English, but support for other languages is being added, and help is welcomed! Check [Translating](#translating) for more info.

[![Crowdin](https://badges.crowdin.net/plakorodb/localized.svg)](https://crowdin.com/project/plakorodb)

Suggestions and corrections are always welcome.

## Copyright

The original game, artwork, logos, card layouts, Japanese text, and all other intellectual property belong to their respective copyright holders.

This repository does **not** claim ownership of those assets.

If the copyright holder requests that any content be modified or removed, I will comply promptly.

## Cards

Translated cards are generated for personal and community use using [**u/Leonarth5's Plakoro Card Maker**](https://leonarthcg.itch.io/plakoro-card-maker).

These cards are provided to make the translation easier to read and reference.

## Contributing

Contributions are welcome!

You can help by:

- reporting translation mistakes
- suggesting more accurate terminology
- adding missing cards (including promotional cards, alternate prints, or corrected versions)
- improving wording or formatting
- providing official translation references when available

And more important, translating the game to other languages! If you're fluent in a langnuage not being supported right now and you want to help, feel free to collaborate!

Feel free to open an Issue or a discussion if you find something missing or want your language included, or make a Pull Request to add to the database!

You can also contact me via discord, by joining [Plakoro Community discord](https://discord.gg/mpVeVj4Ujx). It's a growing community where you will find other people to play with, help with rules, buying, and also me, translating cards there and sharing news.

### Translating

To make translations easier, the project was added to [crowdin](https://crowdin.com/project/plakorodb). Join by clicking the link:

[**Join and help translate!**](https://crwd.in/plakorodb/1ab1323b9058da54873086e6045818a22877741)

If your language is not supported yet, you can request a new language on crowdin's dashboard, or you can ask for it by creating an issue, or writting to u/Jollto.

If your language is supported, I will suggest starting the translation of the [symbols.md](./database/text/symbols.md) and the [move template from wazacards.md](./database/text/wazacards.md#template), and then feel free to translate the moves and the faq and other files that might exist in a future.

To translate, you will have to follow this steps:

- Login to crowdin and join the project.
- Once in the dashboard, select the language you want to work with.
- Select the file you want to translate, and based on the current english translation, you will be able to write the translation.
- Once a translation is finished, you can submit the file for a review request, and a proofreader will check the translation before creating a Pull Request for GitHub.

If you also want to help more, you can ask to be a proofreader and help control new translations for whatever language you want.

Once everything is done, the cards will be translated, and the last step needed will be to create the cards. This probably needs automatization and I'll investigate that when possible, but meanwhile I'll do it manually, or well, you also can, adding the koro files too to the database and making pull requests to add them.

## AI usage in Plakoro Database

AI usage has been kept at a minimum, only used to extract the text from Wazacard spoilers people post online when an OCR program is not enough.

This is my personal (u/Jollto) use. I can't control the contributions nor detect if AI was used, but I will appreciate if this guidelines are followed and we can minimize the use of AI.

All translations are done by hand, trying to base the text effects on the TCG and translating it as often as possible by copying the TCG. Move names are copied from orignal Pokémon moves, either from the videogame or the TCG, and if there is no translation, then I'll try to find a new move name that sounds as good as possible.

### Suggested steps to translate moves

To have an easier time in this process, I do the following steps:

1. Search the japanese move name in [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/Main_Page), it finds all the videogame translations and some of the TCG.
   - If you find it here, easy, copy it and done!
2. Search for the japanese move name in [Pokémon Wiki JP](https://wiki.pokemonwiki.com/wiki/%E3%83%A1%E3%82%A4%E3%83%B3%E3%83%9A%E3%83%BC%E3%82%B8).
   1. If the move exist in TCG, you will find a card here with said move. Open whatever entry and check that the text it found is from the move and not a description.
   2. Search in [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/Main_Page) for that Pokémon card, and copy the translated official name.
      - To search in Bulbapedia for that card, search first the Pokémon name, search in Bulbapedia for that Pokémon TCG (example: Mew TCG) to find all the cards printed for that Pokémon, and using the card number from the japanese wiki, locate the English version of that card, and found! Remember to check that the japanese name you were searching does appear there in Bulbapedia and that you didn't mistakenly found another card.
3. If you still don't find any translations, it will be time to make your own. Here are my tips:
   - Translate the name first using a classic text translator, to get an idea on what you're working.
   - Search for definitions and try to choose a translation that sounds like a Pokémon name.
   - For names with multiple words (like "Fire Wing"), try to find what halves of the japanese word mean each thing, and try to find translations that use that text as a reference.
   - Try not to name the move as something that already exists as that name might get added in a future. To avoid this, after finding a name you like, search for that name in places like Bulbapedia or [cardmarket](https://www.cardmarket.com/en/Pokemon), as that will help you find cards with that name if it already exists. And if that's the case, well, try to find another name.

I also used this to find translations in Spanish, searching first for a TCG card and then finding the localized version. Remember that not all cards have been translated, so maybe it exists in English but not in your language. In that case, follow again the steps above to try and find ideas for the move name.

As the last thing for new names, remember to write a **?** after them in the files, and add it to the list of [original names](/extras/original_names.md).

## License

Unless otherwise noted, my original contributions to this repository are dedicated to the public domain under **CC-BY-NC-4.0**.

This license does **not** apply to either Pokémon's and Plakoro's original artwork, logos, card layouts, or any other copyrighted material owned by their respective rights holders.

## Structure

- [database](/database/) : where you should find what you're searching
  - [cards](/database/cards/) : where to find the cards to print
    - [characards](/database/cards/characards/) : character cards
    - [wazacards](/database/cards/wazacards/) : attack cards
      - [ST](/database/cards/wazacards/ST/): starter set Pokémon
        - one folder for each Pokémon
      - [EB01](/database/cards/wazacards/EB01/) : expansion box 01 Pokémon
        - one folder for each Pokémon
    - [kits](/database/cards/kits/) : prints for each Pokémon with all its cards, plus the .tex files to make them. PDF size is A4, with cards 6cm \* 3 cm.
  - [text](/database/text/) : text translations
    - [symbols.md](/database/text/symbols.md): symbols used by the game, reference here for keys
    - [characards.md](/database/text/characards.md) : characards translation
    - [wazacards.md](/database/text/wazacards.md) : link to files for all Pokémon, for easier access
    - [wazacards](/database/text/wazacards/) : folder for the translated moves
      - [ST](/database/text/wazacards/ST/): starter set Pokémon
        - one file for each Pokémon, with all the moves it has avaiable
      - [EB01](/database/text/wazacards/EB01) : expansion box 01 Pokémon
        - one file for each Pokémon, with all the moves it has avaiable
    - [korocards](/database/text/korocards/): files for the moves to import to Plakoro Card Maker
      - [characards](/database/text/korocards/characards/) : files for the Characards
      - [wazacards](/database/text/korocards/wazacards/) : files for the wazacards, same structure as card images.
    - [faq.md](/database/text/faq.md): Frequently Asked Questions, updated 01/09/2026
- database_XX : database in that language, same structure as above. Files in English unless translated with [Crowdin](#translating)
- [extras](/extras/) : extra files, helpful for the project
  - [icons](/extras/icons/) : images from the official webpage, for Charakoro directions and Enekoro energy.
  - [playseat](/extras/playseat/) : images of translation for the playseat. Contribution made based on Thai Playseat uploaded on the official webpage.
  - [faq_jp.md](/extras/faq_jp.md) : extracted FAQ from original webpage, to use as reference when it gets updated.
  - [orignal_names.md](/extras/original_names.md) : file with names that could not be copied from an official source, and had to get original names. Used to keep control of translations and helpful to mark "checked and approved" translations after talking with the community (still a long work in progress).
