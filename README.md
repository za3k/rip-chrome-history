# rip-chrome-history
Transfer urls and access times from chromium's browser history

Usage: `rip-chrome-history --export export.db`

    Usage: rip-chrome-history [OPTIONS]
        -d|--delete        Delete the database during the rip
        -e|--export FILE   Export the ripped history into the file (appends)
        -f|--file DATABASE Location of the chrome history database [Default: ~/.config/chromium/Default/History]


Rips the Chrome/Chromium browser history database to a unix-friendly file format.
Lines in the export are in this format: `13077638211752775|https://github.com/vanceza/rip-chrome-history`. The number on the left is a unix timestamp.
