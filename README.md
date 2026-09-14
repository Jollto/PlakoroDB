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

## Missing Content

If you notice missing cards (including promotional cards, alternate prints, or corrected versions), feel free to open an Issue with as much information as possible.

## Contributing

Contributions are welcome!

You can help by:

- reporting translation mistakes
- suggesting more accurate terminology
- adding missing cards
- improving wording or formatting
- providing official translation references when available

And more important, translating the game to other languages! If you're fluent in a langnuage not being supported right now and you want to help, feel free to collaborate!

Feel free to open an Issue or a discussion if you find something missing or want your language included, or make a Pull Request to add to the database! 

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

## License

Unless otherwise noted, my original contributions to this repository are dedicated to the public domain under **CC-BY-NC-4.0**.

This license does **not** apply to either Pokémon's and Plakoro's original artwork, logos, card layouts, or any other copyrighted material owned by their respective rights holders.

## Structure

- [database](/database/) : where you should find what you're searching
    - [cards](/database/cards/) : where to find the cards to print
        - [characards](/database/cards/characards/) : character cards
        - [wazacards](/database/cards/wazacards/)  : attack cards
            - [ST](/database/cards/wazacards/ST/): starter set Pokémon
                - one folder for each Pokémon
            - [EB01](/database/cards/wazacards/EB01/) : expansion box 01 Pokémon
                - one folder for each Pokémon
        - [kits](/database/cards/kits/) : prints for each Pokémon with all its cards, plus the .tex files to make them. PDF size is A4, with cards 6cm * 3 cm.
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
        - [faq.md](/database/text/faq.md): Frequently Asked Questions, updated 01/09/2026
