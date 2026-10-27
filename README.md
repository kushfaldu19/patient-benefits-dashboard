# Patient Benefits & EOB Dashboard

A small client-side dashboard using the supplied mock patient, benefit, and EOB data. Patient and EOB pages are navigable via hash routes, including browser back/forward and direct links. No authentication, backend, or installation is required.

## Run locally

From this directory, start a static HTTP server. For example, with Python 3:

```bash
python -m http.server 8000 --directory dist
```

Visit http://localhost:8000. Alternatively, use any static file server that serves `dist/`.

## Structure

- `dist/data.js` — mock patients with nested benefits, EOBs, and analysis.
- `dist/app.js` — routing, formatting, and page rendering.
- `dist/style.css` — responsive layout and styles.
- `dist/index.html` — app shell.

The data is fictional and hardcoded. The analysis repeats the provided mock data and is not a claim adjudication or financial calculation. The difference between billed and allowed amounts is not assumed to be patient responsibility; the values are displayed as provided.

## With more time

Add a backend/API, automated route and component tests, and accessibility testing. Validate financial and denial rules with domain experts and handle additional claim scenarios before using real data.
