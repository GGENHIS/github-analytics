# GitHub Analytics Dashboard

> A sleek, single-page analytics tool that visualises any GitHub user's public activity — stars, commits, languages, and more — right in the browser. No backend, no build step, just open and go.

![GitHub Analytics Preview](https://placehold.co/900x480/0d1117/58a6ff?text=GitHub+Analytics+Dashboard&font=montserrat)

---

## Features

- **Profile overview** — avatar, bio, followers, public repos, and account age at a glance
- **Commit activity chart** — bar chart of contributions over the last year (Chart.js)
- **Top languages** — doughnut chart breaking down language usage across all public repos
- **Stars & forks** — ranked list of most-starred repositories with metadata
- **Repo timeline** — visual history of when each repository was created
- **Dark GitHub-style UI** — pixel-faithful design tokens matching GitHub's own palette
- **Zero dependencies** — one HTML file, CDN-loaded Chart.js, pure Vanilla JS

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, flexbox, grid) |
| Logic | Vanilla JavaScript (ES2020+) |
| Charts | [Chart.js 4.4](https://www.chartjs.org/) |
| Data | [GitHub REST API v3](https://docs.github.com/en/rest) |

---

## Getting Started

### Option 1 — Open directly (recommended)

```bash
# Clone the repo
git clone https://github.com/GGENHIS/github-analytics.git
cd github-analytics

# Open in your browser (no server needed)
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
```

### Option 2 — Serve locally

```bash
# Python 3
python -m http.server 8080

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8080`.

### Usage

1. Enter any GitHub username in the search bar
2. Press **Enter** or click **Analyze**
3. Explore the charts and statistics

> **Note:** The GitHub API allows **60 unauthenticated requests per hour** per IP. If you hit the limit, wait an hour or add a `token` parameter to the fetch headers.

---

## Live Demo

**[github-analytics on GitHub Pages](https://ggenhis.github.io/github-analytics/)**

---

## Project Structure

```
github-analytics/
└── index.html   # Everything — markup, styles, and scripts in one file
```

---

## License

MIT © [GGENHIS](https://github.com/GGENHIS)
