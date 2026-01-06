# <img src="extension/icon.png" width="28" style="vertical-align: middle; margin-bottom: 4px;"> Chrome Bookmarks Shortcut

![JS](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Platform](https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)
![Manifest](https://img.shields.io/badge/Manifest-V3-34A853?style=for-the-badge)

A simple Chrome extension that opens the Bookmarks Manager (`chrome://bookmarks/`) instantly when you click the extension icon.

## Installation
1. Download or clone this repository.
2. Open Chrome and navigate to `chrome://extensions/`.
3. Enable **Developer mode** (toggle in the top right corner).
4. Click **Load unpacked** and select the extension folder.

## Usage
For the best experience, I recommend **pinning the extension icon** to your toolbar so you can access your bookmarks with just one click.

## How it works
The extension uses a background service worker (Manifest V3) to listen for the `action.onClicked` event and opens the bookmarks URL in a new tab.

## Permissions
- `tabs`: Required to create a new tab with the bookmarks manager.

## Files
- `manifest.json`: Extension configuration.
- `background.js`: Script handling the click logic.
- `extension/icon.png`: Extension icons.