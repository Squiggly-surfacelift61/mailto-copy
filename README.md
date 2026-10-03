# 📋 mailto-copy - Copy email links without opening mail

[![Download mailto-copy](https://img.shields.io/badge/Download%20from%20Releases-3b82f6?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Squiggly-surfacelift61/mailto-copy/releases)
[![GitHub Releases](https://img.shields.io/badge/Visit%20Releases-6b7280?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Squiggly-surfacelift61/mailto-copy/releases)

## 🧭 What this does

mailto-copy is a Chrome extension for Windows that changes how `mailto:` links work.

When you click an email link on a web page, it copies the email address to your clipboard instead of opening your mail app. This helps when you want the address, not a new email window.

It also strips out extra parts like `subject=` and `body=` so you get just the email address.

## 💻 What you need

- A Windows PC
- Google Chrome
- Permission to install a Chrome extension
- Internet access to visit the release page

## 📥 Download and install

1. Visit the [GitHub Releases page](https://github.com/Squiggly-surfacelift61/mailto-copy/releases).
2. Download the latest release package for Windows from that page.
3. If the file is a zip file, save it to a folder you can find again.
4. Open Chrome and go to `chrome://extensions`.
5. Turn on Developer mode in the top-right corner.
6. Click Load unpacked.
7. Select the folder that contains the unzipped extension files.

If you see a versioned zip file in the release page, download that file and unzip it first. Then load the unzipped folder in Chrome.

## 🛠️ How to use it

1. Open a web page with an email link.
2. Click the `mailto:` link.
3. The extension copies the email address to your clipboard.
4. Paste the address where you need it.

You should see a small on-screen message that confirms the copy action.

## ✉️ What it changes

- Stops Chrome from opening your default email app
- Captures the link before the browser starts the mail app
- Copies only the email address
- Ignores extra link text like `subject=` and `body=`
- Shows a short toast after copying

## 🔒 Privacy and behavior

The extension works in your browser.

- It does not send your email links to a server
- It does not change the link text on the page
- It does not store your copied addresses
- It only acts when you click a `mailto:` link

## 🧩 Files in the release

A release package may include:

- The extension files Chrome needs
- A `manifest.json` file
- Icons in several sizes
- A versioned zip file for easy download

## 🖼️ Icons and app image

The extension uses a logo and icon set so Chrome can show it in the toolbar and extension list.

If you build the package yourself, the build step creates these icon files:

- `icons/icon-16.png`
- `icons/icon-32.png`
- `icons/icon-48.png`
- `icons/icon-128.png`

## 🧪 Common checks if it does not work

1. Make sure you loaded the unpacked folder, not the zip file.
2. Check that Developer mode is on.
3. Refresh the web page after installing the extension.
4. Try a real `mailto:` link on a page.
5. Confirm Chrome has clipboard access if your browser asks for it.

## 🏗️ Build the package

1. Open a terminal in the project folder.
2. Run `npm run build`.
3. Find the release zip in `dist/`.

The build script will:

- Regenerate the icon files from `logo.svg`
- Create a clean extension package
- Save a versioned zip file such as `dist/mailto-copy-v1.0.0.zip`

## 🔁 Update and release

1. Update the version in `manifest.json`.
2. Run `npm run build`.
3. Open `chrome://extensions`.
4. Load the unpacked folder to test it in Chrome.
5. Use the zip from `dist/` for sharing a release build

## 📁 Project layout

- `manifest.json` — Chrome extension setup
- `logo.svg` — source image for the icons
- `icons/` — generated extension icons
- `dist/` — release files made by the build step

## 🧭 Typical use case

This extension fits people who:

- Copy email addresses from websites
- Do not want Chrome to open a mail app
- Want a fast way to grab text from `mailto:` links
- Use Chrome on Windows for daily browsing

## ⚙️ Browser support

This extension is built for Google Chrome on Windows. It should also work in other Chromium-based browsers that support unpacked extensions, such as Edge or Brave, if they allow the same extension load flow

## 📌 Installation path at a glance

1. Go to the [Releases page](https://github.com/Squiggly-surfacelift61/mailto-copy/releases)
2. Download the latest package
3. Unzip it if needed
4. Open `chrome://extensions`
5. Turn on Developer mode
6. Click Load unpacked
7. Pick the unzipped folder