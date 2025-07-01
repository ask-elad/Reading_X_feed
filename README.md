# 🌐 X Feed Xchange – See the World Through Their Feed

**X Feed Xchange** is a Firefox browser extension that lets you simulate the Twitter (X) home feed of another public user — in a safe, **read-only** mode.  
No likes. No replies. Just the raw feed — as they see it.

> 🔒 Designed for ethical use only — ideal for developers, researchers, and hackathon demos.

---

## 🧐 What Is It?

Twitter (X) generates a personalized feed for every user based on who they follow, like, mute, and interact with.  
This extension allows you to:

- View another user’s home feed using their session tokens
- Do so **without logging in** or interacting with the platform
- Browse in a completely **read-only environment**

> Think of it like “View Only” mode in Google Docs — but for X feeds.

---

## 🔧 Features

- ✅ Copy your own Twitter session tokens (auth + CSRF)
- ✅ Input another user’s tokens (with their permission)
- ✅ Load their home timeline inside Firefox
- ✅ Hide distracting UI (sidebars, tweet boxes, etc.)
- ✅ Disable all interactions (retweets, likes, replies)
- ✅ Fully read-only and safe for demo or research use

---

## 🖼️ Demo Preview

> Enter your tokens or a friend’s to load the feed in read-only mode.

- All buttons like Like, Retweet, Reply are disabled
- You see exactly what the other person would see
- UI is stripped down for focused viewing

---

## 🚀 Installation

### 🔧 Load Temporarily in Firefox

1. Open Firefox and go to: `about:debugging#/runtime/this-firefox`
2. Click **“Load Temporary Add-on”**
3. Select the `manifest.json` file in your extension folder

> ⚠️ This loads the extension temporarily — it will disappear after you restart Firefox.

---

### 📦 Install Permanently via AMO (Mozilla Add-ons)

1. Create a `.zip` of your extension folder
2. Go to: [https://addons.mozilla.org/en-US/developers/](https://addons.mozilla.org/en-US/developers/)
3. Sign in and **Submit a New Add-on**
4. Choose **Listed** (for public use) or **Unlisted** (for private installs)
5. Upload your `.zip`, fill in metadata, and wait for approval

---

## 📁 Project Structure

x-feed-xchange/
├── popup.html → Extension popup interface
├── popup.js → Token handling logic
├── content.js → Applies read-only logic to feed
├── background.js → Sets cookies & restores sessions
├── manifest.json → Firefox extension configuration
├── popup.css → Simple styling
└── images/icon.png → Extension icon
