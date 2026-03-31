## 📝 Markdown Editor/Viewer

A fast, fully responsive, and completely client-side Markdown editor built into a single HTML file. Markdown Editor/Viewer provides real-time previews, offline capabilities, and native OS integrations—all without needing a backend or complex build step.

## ✨ Features

Single-File Architecture: The entire app (HTML, CSS, JS, and PWA assets) is contained within a single index.html file. Just drop it anywhere and it works.

Real-Time Preview: See your markdown rendered as you type, complete with GitHub Flavored Markdown (GFM) support.

Secure Local Storage: Your work is automatically saved to your browser's IndexedDB using localstorage. No data ever leaves the device.

Progressive Web App (PWA): Install it as a standalone app on your desktop or mobile device. (Dynamically generates its own manifest and service worker).

Native OS File Handling: Once installed as a PWA on supported OSs (like Windows), right-click .md or .txt files and select "Open with Markdown Studio".

Responsive Design: Side-by-side editing on desktop, and a smooth, toggle-based full-screen experience on mobile devices.

Synchronized Scrolling: The preview pane intelligently scrolls to match your position in the editor.

Built-in Print Support: Clean, distraction-free printing that isolates the rendered document.

Markdown Help Guide: A quick-reference cheat sheet for standard Markdown syntax.

## 🚀 Getting Started


Option 1: Quick Run (View Only)

Simply download index.html and double-click it to open it in your browser (file:/// protocol).
Note: The core editor will work perfectly, but browser security restrictions prevent PWA installation and native OS file-handling from file:/// URLs.

Option 2: Full Experience (Local Server)

To unlock PWA installation and File Handler APIs, you need to serve the file over localhost or https://.

Clone this repository or download index.html.

Serve the directory using a local web server. For example:

Python: python -m http.server 8000

Node.js: npx serve .

VS Code: Use the "Live Server" extension.

Open http://localhost:8000 in your browser.

Click the Install App button (or the install icon in your browser's address bar) to install it to your system.

## 🛠️ Tech Stack

This project utilizes modern web standards and lightweight libraries delivered via CDN:

Styling: Tailwind CSS

Icons: Lucide Icons

Markdown Parsing: Marked.js

Security/Sanitization: DOMPurify

Local Storage: LocalForage

## 🔒 Security

All Markdown input is passed through DOMPurify before being rendered to the screen to prevent Cross-Site Scripting (XSS) attacks. Additionally, no data is ever transmitted over the network; everything is kept strictly on your local device.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details. 
