# CV — cv.protcenko.com

  Source for my personal CV / portfolio site: **[cv.protcenko.com](https://cv.protcenko.com)**

  A single, self-contained `index.html` — no build step, no framework, no runtime
  dependencies. Deployed via GitHub Pages on a custom domain.

  ## Highlights
  - **Two-layer design tokens** (primitive palette → semantic roles) driving a
    light/dark theme with a single source of truth.
  - **Flash-free theming** — theme is resolved in a synchronous head bootstrap
    before first paint; respects stored preference and `prefers-color-scheme`.
  - **Accessible & progressive** — semantic HTML landmarks, keyboard-visible skip
    link, `prefers-reduced-motion` support, JSON-LD structured data, graceful
    no-JS fallback.
  - **Dynamic CV generation** — the "Download CV (PDF)" button builds an
    ATS-friendly, selectable-text PDF *from the live page content* at click time
    (jsPDF, lazy-loaded). Edit the page, the CV follows — nothing to keep in sync.

  ## Structure
  index.html                 # the entire site (HTML + inlined CSS + JS)
  vendor/jspdf.umd.min.js     # self-hosted PDF library (lazy-loaded on demand)
  og-image.png                # social share card
  apple-touch-icon.png        # iOS home-screen icon
  CNAME                       # custom domain
