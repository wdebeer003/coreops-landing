# CoreOps Landing Page

The public marketing site for CoreOps — a static site, no build step, deployed via GitHub Pages.

## Structure

- `index.html` — the homepage. All content is sourced from the CoreOps discovery deck
  (`docs/discovery-deck.html` in the main `hospitality-os` app repo), which is itself
  fact-checked against the live product codebase — don't add feature claims here that
  aren't already verified there.
- `styles.css` — shared stylesheet. Matches the CoreOps app's own theme: zinc-950
  background, emerald accent, glass-morphism cards. Any future page (`pricing.html`,
  `features.html`, etc.) should reuse this file and the same header/footer markup rather
  than starting a new design.
- `favicon.svg` — the CoreOps logo mark.
- `.nojekyll` — disables GitHub Pages' default Jekyll processing, since this is plain
  static HTML/CSS with no Jekyll front matter.

## Deploying

Pushed to `main` → GitHub Pages (Settings → Pages → Deploy from branch → `main` → `/`)
serves it directly. No build step.

## Note on the old hos-landing repo

This repo intentionally replaces `hos-landing` rather than reusing it. `hos-landing`'s
GitHub Pages URL was shared with someone before this rename — since GitHub Pages has no
access control, redeploying under that same URL would have shown the new CoreOps content
to that old recipient too. `hos-landing` is left untouched; this is a fresh repo with a
fresh URL.
