# LC Express 14U — Team Website

Static site (single `index.html`) for LC Express 14U Fastpitch Softball, Normangee, TX.
Content is managed from a Google Sheet; the page reads it in the browser on each visit.

## Data
The site reads **LC Express 14U | Website Feed (Public)** (`CONFIG.SHEET_ID` in `index.html`).
That feed pulls from the coach's private master sheet (*LC Express 14U | Recruiting Master Database*) with IMPORTRANGE:

- **Players**: only rows marked `Yes` under "Public Approved?", and only public columns (no approval status, no parent contacts).
- **Games, Tournaments, Settings**: copied as-is.

The feed sheet must be shared as "Anyone with the link: Viewer". The master sheet stays private.
Headshots: drop `assets/players/<profile-slug>.webp` in the repo; otherwise the Drive photo link is tried, then a silhouette.

## Pages (hash routes)
`#home` `#roster` `#player-first-last` `#schedule` `#tournaments` `#about` `#recruiting` `#card` `#contact`

Built and maintained by V8 Technologies.
