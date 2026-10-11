# money

A personal budgeting page served by GitHub Pages: payday flow, monthly plan, check-ins, goals and a to-do list.

This repository holds **no personal data**. The page is a shell. On first use on each device it asks for a fine-grained GitHub token that can read and write one private repository, and it loads and saves a single `data.json` there through the GitHub API. Every save is a commit, so the private repo's history is the full record.

Security notes:
- The token is kept in the browser's local storage on that device only and is sent nowhere except `api.github.com`.
- A Content Security Policy limits network access to `api.github.com` (plus Google Fonts for type).
- No third-party scripts. The page is set to `noindex`.
