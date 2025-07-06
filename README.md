# auto-unmute-x-com-userscript

A tiny userscript that automatically unmutes autoplayed videos on [x.com](https://x.com) (formerly Twitter). It does **not** adjust volume levels—just unmute—and does **not** leave a focus ring (no blue border) after unmuting.

## Features

- Automatically unmutes any `<video>` element on play  
- Zero dependencies—pure vanilla JS  
- MutationObserver-based: binds to videos as they appear  
- Does **not** focus the video element, so no blue outline appears  
- Automatic updates via GitHub raw URLs

## Installation

1. Install a userscript manager:
   - [Tampermonkey (Chrome, Edge, Safari, Opera)](https://www.tampermonkey.net/)  
   - [Greasemonkey (Firefox)](https://addons.mozilla.org/firefox/addon/greasemonkey/)  
2. Install the script by visiting the raw URL:
   ```
   https://raw.githubusercontent.com/M19-ca/auto-unmute-x-com-userscript/main/x-auto-unmute.user.js
   ```
3. Confirm installation when prompted.

## Usage

Once installed, the script will:

1. Watch for any `<video>` elements on pages under `https://x.com/*`  
2. As soon as a video begins playback, remove its `muted` flag  
3. Leave the page’s normal focus behavior untouched—no blue border appears  

There are no settings or menu toggles. To disable, simply turn off or uninstall the script in your userscript manager.

## Development

```bash
git clone https://github.com/M19-ca/auto-unmute-x-com-userscript.git
cd auto-unmute-x-com-userscript

# Edit x-auto-unmute.user.js to make changes
git add x-auto-unmute.user.js
git commit -m "Describe your change"
git push
```

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for full text.

