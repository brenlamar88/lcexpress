# LC Express 14U — Team Website

Static site (single `index.html`) for LC Express 14U Fastpitch Softball, Normangee, TX.
Content is managed from a Google Sheet; the page reads it in the browser on each visit.

## Going live with the Google Sheet
1. Sheet tabs: `Settings`, `Players`, `Games`, `Tournaments`, `Coaches` (see `LC_Express_Website_Data.xlsx` template).
2. Format all cells as Plain text. Share → "Anyone with the link" → Viewer.
3. In `index.html`, set `CONFIG.SHEET_ID` to the ID from the sheet URL and `CONFIG.SITE_URL` to the final domain (used in QR codes).

Until `SHEET_ID` is set, the site shows built-in sample data.

## Pages (hash routes)
`#home` `#roster` `#player-first-last` `#schedule` `#tournaments` `#about` `#recruiting` `#card` `#contact`

Built and maintained by V8 Technologies.
