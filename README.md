# Compact Discord

Collapse the member and channel lists on small screens to save space.

Member list collapses at 1024px, Channel list collapses at 768px.

[![Install in Replugged](https://img.shields.io/badge/-Install%20in%20Replugged-blue?style=for-the-badge&logo=none)](https://replugged.dev/install?identifier=asportnoy/compact-discord&source=github)

![Demo](demo.gif)

## TIP: allow Discord to be resized to any size

1. Open the Discord settings.json file

   - Windows: `%APPDATA%/discord/settings.json`
   - MacOS: `~/Library/Application Support/discord/settings.json`
   - Linux: `~/.config/discord/settings.json` (may vary depending on Discord location)

   For other platforms (besides stable) you will need to replace `discord` with the appropriate
   folder name. It could by hyphenated (like `discord-canary`) or not (like `discordcanary`).

2. Set the properties `MIN_WIDTH` and `MIN_HEIGHT` to `0`. The file should look like this:

   ```json
   {
     "IS_MINIMIZED": false,
     "MIN_WIDTH": 0,
     "MIN_HEIGHT": 0,
     "WINDOW_BOUNDS": {
       "x": 500,
       "y": 25,
       "width": 940,
       "height": 875
     },
     "BACKGROUND_COLOR": "#202225"
   }
   ```

3. Fully quit and restart Discord
