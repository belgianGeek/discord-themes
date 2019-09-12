# How to install and use the themes

This project's themes use _Betterdiscord_, a piece of software allowing you to extend the features of your Discord client with plugins (you can for example quote messages, encrypt channels...) and themes (like this project).

If you don't have it installed yet, I advise you to install more specifically _BandagedBD_, a _Betterdiscord_ fork made by Rauenzi. It is available [here](https://github.com/rauenzi/BetterDiscordApp/releases). _BandagedBD_ is fully compatible with Windows and MacOS. If you run Linux, you will have to deal with the `.tar.gz` archive or , if you are lucky, it is already suppported by your package manager.

Once _BandagedBD_ is installed, reload Discord (`ctrl + R` on Windows and Linux) so to apply your config changes. To know if Discord has detected _BandagedBD_, just open the Discord settings : a new section named `BandagedBD` had to be added to the existing settings list. If this is not the case, restart Discord until it comes up, or reinstall _BandagedBD_.

To install the theme(s) of your choice, you just have to download the `.theme.css` file you want. Once done, have a look in the Discord settings, in the newly added _Themes_ section and click on the button _Open theme folder_. Paste the theme(s) you have downloaded in the opened explorator window.

To (de)activate a theme, just click on the button next to each theme's name. Once a theme is activated, the Discord interface should automatically adapt itself to the new config.

# Customize an existing theme

You're not satisfied with these themes (previews are available [here](https://framagit.org/Leroux47/discord-themes/tree/master/images)) ?
Don't worry, the customization is EXTREMELY easy.

First of all, head over the Discord settings, in the _Custom CSS_ menu.

## Modify the global appareance (colors, fonts...)

1. `--mainColor: <color>` : modify the main colors of the interface (titles, buttons, checkboxes, guild names background...).
2. `--secondColor: <color>` : applies to the buttons backrgound and to the guild names on hover.
3. `--thirdColor: <color>` : change the background color of the channels names, the friends list and the guild members list.
4. `--fourthColor: <color>` and `--fifthColor: <color>` : modify the settings and popup windows background color.
4. `--font: <font_name>` : modify the font used in Discord. This rule needs to be used with a `@import url(<font_url>)` statement, explained below.
5. `--textColor: <color>` : change the font color (almost) everywhere in Discord.

:sparkles: The `1.3.0` release introduced new rules to make customization easier :

- `--fouthColor: <color>` and `--fifthColor: <color>` : add a background to the settings submenus, users profile, etc.
- `--backgroundImage: url(<image_url>)`: modify the background image.
- `--buttonColor: <color>`: change the toolbar buttons color.
- `--homeIcon: url(image_url>)`: change the background image of the Discord _Home_ button (in the upper left corner of the Discord interface).
    ⚠ The chosen icon size must be at most 50x50 px.

All those rules (except the `@import`, which has to be the first, out of any rules group) must be placed inside a statements block like the following :

:root {
    rule1 : <value>;
    rule2 : <value>;
    }

## Modify the font style

A bit more complicated... 😁 First, you must know which font you want to use. Then, verify if it's available via [Google fonts](https://fonts.google.com) or [a equivalent](https://alternativeto.net/software/google-web-fonts/).

Once done, you can import your font thanks to a rule you can add in the _Custom CSS_ input box, like this :

    @import url(<font_url>);

    :root {
        --font : <font_name>;
    }

You can change the text color using the `--textColor: <color>` rule.

## Modify the background color/image

You can use this schema :

body {
    background-image: url(<image_url>);
    background-color: <color>;
}

😉 Since the `1.3.0` release, these rules can be replaced by this : `--backgroundImage: url(<image_url>)`.

Please note you can only use one of these rules at the same time.

# Contribute

You can contribute to this project by suggesting enhancements (open an issue, suggest a pull request...) on GitHub/GitLab or by email.

# You have an issue/question ?

Raise an issue or feel free to contact me.

# License

All this repo is licensed under the GNU GPL v3, except the project's avatar, which comes from [here](https://www.iconfinder.com/icons/1542372/discord_media_social_icon).
