# stardew-predictor

## About Stardew Predictor

This app simulates the random number generator used in [Stardew Valley](https://stardewvalley.net/) and makes "predictions" about the game either from the Game ID or by reading the save file. Currently, the information predicted includes special mine levels (e.g. mushroom floor &amp; infestations), random items sold by some vendors, results from cracking geodes, the train schedule, and more.
A useful companion tool is [BlaDe's Map Predictor](https://www.nexusmods.com/stardewvalley/mods/6614) which handles things such as artifact digging, giant crops, and mine ladders.

All changed & added content from version 1.6 should be supported; 1.6-specific features will only appear in the results if either the save is detected to be from that version or the app is launched with a URL id parameter.

The app is written in Javascript and uses [jQuery](https://jquery.com/), [BigInteger.js](https://github.com/peterolson/BigInteger.js), [JS xxHash](https://github.com/pierrec/js-xxhash), and [pako](https://github.com/nodeca/pako); it is hosted on GitHub Pages at https://mouseypounds.github.io/stardew-predictor/ and the source code repository is https://github.com/MouseyPounds/stardew-predictor. It is released under the MIT license.

Please report any bugs, suggestions, or other feedback to [the topic in the Stardew official forums](https://forums.stardewvalley.net/threads/web-apps-stardew-checkup-predictor-and-fair-helper.28393/) or to @mouseypounds on Discord.

## Changelog

* 20 Apr  2024 - v5.0.8 - Fixed advanced usage breaking after last update; better mp sanity-checking
* 18 Apr  2024 - v5.0.7 - One more seed overflow fix, changes for patch 1.6.4, support for compressed Switch saves
*  7 Apr  2024 - v5.0.6 - Variety of PR bugfixes
*  6 Apr  2024 - v5.0.5 - Bugfix for invalid ID in URL; marked Sandy shirts that are otherwise hard to acquire
*  4 Apr  2024 - v5.0.4 - Bugfixes for Prize Tickets, first 10 mystery boxes, and Calico Jack dealer draws
* 30 Mar  2024 - v5.0.3 - Finally added slightly more friendly error-handling
* 28 Mar  2024 - v5.0.2 - Fixed precision loss bug in enchantment code
* 27 Mar  2024 - v5.0.1 - Update cart item lists for 1.6.3 patch
* 26 Mar  2024 - v5.0.0 - Support for Stardew Valley 1.6
* 15 Jan  2021 - v4.0.4 - Updating Night event chances for Stardew Valley 1.5.3
*  9 Jan  2021 - v4.0.3 - No code changes, only clarifications on some mechanics.
* 30 Dec  2020 - v4.0.2 - Made geode fix only apply to 1.5 saves
* 28 Dec  2020 - v4.0.1 - Fixed geode predictions
* 22 Dec  2020 - v4.0   - Initial support for Stardew Valley 1.5
* 24 Jul  2020 - v3.1.3 - Updated forum link in footer
*  6 Mar  2020 - v3.1.2 - Fixed Krobus search
*  1 Feb  2020 - v3.1.1 - Fixed one of the white eggs in the cart prediction being incorrectly listed as brown. (Thanks rickselby)
* 29 Dec  2019 - v3.1.0 - Added Skull Cave Dino levels to Mine info and a new tab for Garbage Can loot; also some fixes and formatting changes
* 13 Dec  2019 - v3.0.3 - Another small version error regarding artifact troves in search results
*  7 Dec  2019 - v3.0.2 - Version detection changed again to handle semver like 1.4.2
* 30 Nov  2019 - v3.0.1 - Version detection should now properly identify day one 1.4 saves
* 26 Nov  2019 - v3.0   - Support for Stardew Valley 1.4
*  5 July 2019 - v2.2.1 - Fixed a wiki link error.
* 30 Jan  2019 - v2.2   - Improved support for iOS save files
* 24 Oct  2018 - v2.1   - Added Wallpaper predictions and moved images to spritesheets
*  3 Oct  2018 - v2.0.2 - Bug fixes for Winter Star processing when using URL ID parameter instead of a save
*  1 Sept 2018 - v2.0.1 - Collapse older entries in changelog
* 20 Aug  2018 - v2.0   - Added Krobus tab (thanks ronw23 on GitHub). Better input sanitization for anti-Cat protection
* 18 Aug  2018 - v1.8   - Added public domain BigInteger library; MP support and fixed predictions for Winter Star 1.3
* 17 Aug  2018 - v1.7.1 - Added warning about broken Winter Star predictions in 1.3
* 17 Aug  2018 - v1.7   - Small bugfix on Geode predictions for 1.3
* 24 May  2018 - v1.6   - Favicon; Baby question for 1.2 save night events
* 23 May  2018 - v1.5.1 - Clarification in Night event intro & disclaimer about 1.2
* 21 May  2018 - v1.5   - Night events added; list potential Winter Star gifts
*  7 May  2018 - v1.4   - Geode counter bugfix; additional multiplayer support
*  6 May  2018 - v1.3   - Traveling Merchant now includes Night Market if save is from 1.3
*  4 May  2018 - v1.2   - Days Played bugfix
* 14 Apr  2018 - v1.1   - Train schedule added
*  7 Mar  2018 - v1.0   - Full release, searching for geodes added
*  4 Mar  2018 - v0.94  - Rewrite of RNG class to avoid ES2015-specific features for Pale Moon compatibility
*  3 Mar  2018 - v0.93  - Indicator for geode contents which need donation
* 25 Feb  2018 - v0.92  - Fixing Baryte spelling and double-button processing bug
* 22 Feb  2018 - v0.91  - Search for Cart items, Winter Star bugfix
* 20 Feb  2018 - v0.9   - Beta Testing
*  4 July 2017 - v0.5   - Alpha Testing