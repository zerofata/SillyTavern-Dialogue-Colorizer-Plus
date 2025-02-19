# SillyTavern Dialogue Colorizer

This is a fork of [XanadusWorks/SillyTavern-Dialogue-Colorizer](https://github.com/XanadusWorks/SillyTavern-Dialogue-Colorizer) with minor improvements.

## Improvements
- Assigns character colours to a CSS variable '--character-color' so that it can be used in custom css. Scoped to the .mes element to support group chats.

![image](https://github.com/user-attachments/assets/0dbfd4a9-929a-4393-b436-cf3dc0d1d6cd)


```css
.mesAvatarWrapper .avatar {
    margin-bottom: 8px;
    outline-offset: 3px;
}
/* Avatar Icon */
div.mes .mesAvatarWrapper .avatar, div.mes .mesIDDisplay:not(:empty), div.mes .mes_timer:not(:empty), div.mes .tokenCounterDisplay:not(:empty) {
    outline: 1px solid var(--character-color);
    box-shadow: 0px 0px 2px 1px rgb(from var(--character-color) r g b / 80%);
}
/* MessageID, Timer & Token Displays */
div.mes .mesIDDisplay:not(:empty), div.mes .mes_timer:not(:empty), div.mes .tokenCounterDisplay:not(:empty) {
    outline: 1px solid var(--character-color);
    outline-offset: -1px;
    box-shadow: 0px 0px 1px 1px rgb(from var(--character-color) r g b / 20%);
}
```

## Installation and Basic Usage
Use ST's built-in third-party extension installer. Enter this repository's URL in the Extensions tab under "Install Extension".

For detailed usage instructions and features, see the [original repository](https://github.com/XanadusWorks/SillyTavern-Dialogue-Colorizer).

## License
MIT License - see [LICENSE](./LICENSE)
