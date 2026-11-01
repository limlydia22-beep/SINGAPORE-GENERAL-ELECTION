# Singapore General Election Results (GE2015, GE2020, GE2025)

A static, single-page web app. No build step and no dependencies: everything (code, styles and data) is inside `index.html`.

## Deploy on Vercel
Option A — drag and drop: go to https://vercel.com/new, choose to deploy without Git (or use "Upload"), and drop this folder.
Option B — CLI: `npm i -g vercel`, then run `vercel --prod` inside this folder.
Option C — Git: push this folder to a GitHub repo and import it at https://vercel.com/new. Framework preset: "Other". Leave build command and output directory empty.

## Files
- `index.html` — the app (data embedded).
- `data.json` — the same results data on its own, for reference or reuse. The app does not load it.
- `vercel.json` — clean URLs and basic security headers. Optional; the site also works without it.

## Data source
Elections Department Singapore (ELD), "Parliamentary General Election Results by Candidate", via data.gov.sg
(https://data.gov.sg/datasets/d_581a30bee57fa7d8383d6bc94739ad00/view). The GE2025 Marine Parade-Braddell Heights GRC walkover (PAP, 5 seats) is not in that dataset and was added by hand. Please check important figures against https://www.eld.gov.sg.
