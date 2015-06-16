# rip-chrome-history
Transfer urls and access times from chromium's browser history

Example: `rip-chrome-history --export export.db`

    Usage: rip-chrome-history [OPTIONS]
        -d|--delete        Clear the database during the rip, so that append-mode rips won't duplicate data. If chrome/chromium is in use, the rip will succeed but the file will not be deleted.
        -e|--export FILE   Export the ripped history into the file (appends)
        -f|--file DATABASE Location of the chrome history database [Default: ~/.config/chromium/Default/History]

Rips the Chrome/Chromium browser history database to a unix-friendly file format.
Lines in the export are in this format: `13077638211752775|https://github.com/vanceza/rip-chrome-history`. The number on the left is a unix timestamp.
