# cnyprogress-site

Static port of the Google Site `sites.google.com/view/cnyprogress` (Sunny Aslam, MD),
rebuilt as plain HTML + CSS with no build step, ready for GitHub Pages.

## Structure

- `index.html` — homepage
- `styles.css` — shared stylesheet (system fonts, no external dependencies)
- `about-me/` — about page
- `ai-safety/` — AI safety page
- `addiction-and-access/` — addiction & clinical work page
- `community-advocacy/` — community advocacy page
- `cny-medical-debt/` — medical debt project page
- `news-updates/` — commentary and updates (includes Oct 2026 county-study bullet)
- `data-center-deals/` — data center negotiation toolkit landing page
  - `principles/` — 10-principle negotiating framework (unattributed)
  - `term-sheet/` — 30-point model term sheet (unattributed)
  - `comparables/` — U.S. deal comparison table (unattributed)
  - `source-library/` — primary-source library (copied interactive page, verbatim)
  - `10-questions/` — 10 questions for a public hearing (copied, verbatim)
  - `scorecard/` — proposal scorecard tool (copied, verbatim)
  - `who-decides-what/` — NY roles explainer (copied, verbatim)
  - `files/` — PDF and Word downloads of the toolkit documents

The three policy documents (principles, term sheet, comparables) intentionally carry
no name, no bio, and no attribution, per the owner's standing preference.

## Conventions

- Relative links only (`../styles.css` etc.), so the site works from any base path,
  including GitHub Pages project sites (`username.github.io/repo/`).
- Every page carries `<!-- ANALYTICS: paste GA4 snippet here -->` in `<head>`.
- `<!-- TODO: ... -->` comments mark external URLs that could not be recovered
  from the old site (article links, LinkedIn, Upstate profile, PubMed, PBS).
  Fill these in before or after publishing.

## Publishing checklist (for the site owner)

1. Create a GitHub repo, add it as remote, push.
2. Enable GitHub Pages (Settings → Pages → Deploy from branch → main → / (root)).
3. Optional: custom domain (~$10–15/yr) via DNS; enforce HTTPS in Pages settings.
4. Add the GA4 measurement ID at each `ANALYTICS` placeholder.
5. Fill in the `TODO` external URLs.
6. Update old LinkedIn posts to point at the new URLs.

## Local preview

    cd ~/workspace/cnyprogress-site && python3 -m http.server 8000
