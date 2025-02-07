# /tellraw Command Guide

The `/tellraw` command in Minecraft allows you to send a customized, colored message to a player.

### Syntax for Sending a Colored Message:

### Example:
To send the message "Test" to yourself (`@s`) in green color, use the following command:
/tellraw @s {"text":"Test", "color":"#00ff00"}

### Parameters:
- **$player$**: The player to whom the message is sent. Example: `@s` (yourself), `@a` (all players), `@p` (nearest player), etc.
- **$text$**: The message you want to display. Example: `"Test"`.
- **$color$**: The color of the text. This can be a color name or a hex code. Example: `"red"`, `"blue"`, or `"#00ff00"` (green).

### Color Options:
- `"black"`
- `"dark_blue"`
- `"dark_green"`
- `"dark_aqua"`
- `"dark_red"`
- `"dark_purple"`
- `"gold"`
- `"gray"`
- `"dark_gray"`
- `"blue"`
- `"green"`
- `"aqua"`
- `"red"`
- `"light_purple"`
- `"yellow"`
- `"white"`
- Hex codes (e.g., `#00ff00` for green).

### Additional Formatting Options:
You can also use additional formatting like **bold**, **italic**, **underlined**, etc.

- **Bold**: Add `"bold": true`
- **Italic**: Add `"italic": true`
- **Underlined**: Add `"underlined": true`
- **Strikethrough**: Add `"strikethrough": true`
- **Obfuscated**: Add `"obfuscated": true`

### Example with Formatting:
To send a bold, red message to yourself, use:
/tellraw @s {"text":"Test", "color":"red", "bold":true}

To send an italic, green message to yourself, use:
/tellraw @s {"text":"Test", "color":"green", "italic":true}

Feel free to adjust the text and color values as needed for your server or gameplay experience.

