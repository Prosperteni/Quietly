<div align="center">

<img src="icons/icon128.png" alt="Quietly icon" width="96" />

# Quietly

**Automatic YouTube ad muter — silent ads, seamless viewing.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Platform: Chrome](https://img.shields.io/badge/Platform-Chrome-yellow.svg?style=flat-square&logo=googlechrome&logoColor=white)](https://chrome.google.com/webstore)
[![Manifest: V3](https://img.shields.io/badge/Manifest-V3-green.svg?style=flat-square)](manifest.json)
[![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen.svg?style=flat-square)]()

</div>


**Quietly** is a Chrome extension that automatically detects YouTube ads and mutes them in real time and then restores audio for normal video playback.

It runs entirely on the client side and requires no external servers.

---

## Features

- ✅ Automatically mutes YouTube ads  
- ✅ Restores audio when the ad ends  
- ✅ Works across multiple YouTube tabs  
- ✅ Persists ON/OFF state across browser sessions  
- ✅ Real-time detection using DOM monitoring  
- ✅ Robust ad detection using multiple conditions  
- ✅ Lightweight and fast (runs every 500ms)

---

## How It Works

### Message Flow
1. User clicks **Enable/Disable** in the popup  
2. `popup.js` sends a message to `background.js`  
3. Background updates Chrome storage  
4. Background notifies all open YouTube tabs  
5. `content.js` reacts and starts/stops muting ads  

---

## Project Structure
```bash
Quietly/
│
├── manifest.json
├── background.js
├── content.js
│
├── popup/
│ └── popup.html
│ └── popup.js
│
└── icons/
├── icon16.png
├── icon32.png
├── icon48.png
└── icon128.png
```
---

## Installation (Developer Mode)

1. Open **Chrome**
2. Go to:  chrome://extensions/
3. Enable **Developer mode** (top right)
4. Click **Load unpacked**
5. Select this project folder

---

## Permissions Used

- `activeTab` – communicate with current tab  
- `scripting` – content script injection  
- `storage` – save ON/OFF state  

---

## Limitations

- YouTube UI changes may break selectors temporarily  
- Does not block ads visually — only mutes them  
- Requires a refresh if YouTube changes major structure  

---

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on how to get started, including branching, commit message formatting, and local testing.

---


<div align="center">

**Built for smarter YouTube viewing.**

</div>
