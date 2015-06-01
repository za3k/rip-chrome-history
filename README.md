# rip-chrome-history
Transfer urls and access times from chromium's browser history

Usage: `rip-chrome-history export.db`

Rips the Chrome/Chromium browser history database to a unix-friendly file format. This command deletes the history database (unless Chrome/Chromium is in use), but only appends to the export file.
Lines in the export are in this format: `13077638211752775|https://github.com/vanceza/rip-chrome-history`
