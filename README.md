#PARKSPOT
Dependencies & Setup
Runtime & System Requirements
Node.js (v18+ or LTS recommended)

npm (included with Node.js)

Modern Web Browser (Chrome, Brave, Edge, or Firefox with JavaScript and localStorage enabled)

Node.js Packages
Your backend relies on Node.js with Express for HTTP routing/static file serving, Socket.IO for real-time updates, and SQLite for local database storage (parkspot.db).

Install dependencies from the parkspot directory using:

Bash
npm install
Typical core packages used in this stack include:

express — Web server and static asset delivery (public/)

socket.io — Real-time bidirectional slot and occupancy updates

SQLite driver (such as sqlite3 or better-sqlite3, depending on your package.json) — Local database persistence (parkspot.db)

(If you ever set up a fresh package.json from scratch, check your existing package.json first so the exact SQLite package name matches db.js.)

Frontend Assets (No Build Step)
The frontend uses vanilla HTML, CSS, and JavaScript served from public/:

Socket.IO Client — Automatically served by the backend at /socket.io/socket.io.js

Google Fonts (Barlow and Barlow Condensed) — Loaded via <link> in index.html

Running Locally
Open a terminal in the project folder (parkspot).

Install packages:

Bash
npm install
Start the server:

Bash
node server.js
Open http://localhost:3000 in your browser.
