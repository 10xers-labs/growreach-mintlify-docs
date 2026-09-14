<!-- EDIT LOG — one line per create/edit event. Session name + ID let you resume the exact chat that did the work. -->
<!-- created: setup mintlify | 20260910_100433_f78983 | 2026-09-10 12:07 UTC -->
# Contributing to the GrowReach Help Center

This repository is the source for the GrowReach help center, deployed to Mintlify. Every push to `main` auto-deploys the site.

## Two ways to edit

### 1. GitHub (recommended)

1. Edit the `.mdx` files in this repo.
2. Open a pull request.
3. Merge — the site auto-deploys.

### 2. Mintlify web editor

1. Go to the [Mintlify dashboard](https://app.mintlify.com) and open the editor.
2. Edit a page.
3. Click **Publish** — changes ship as a pull request (or direct push, depending on branch protection).

## Content rules

- **No competitor comparisons** — never mention other tools by name, no "vs X" pages, no comparison tables.
- **No confidential material** — no internal docs, prompts, or implementation details.
- **No third-party tool links** — the docs are self-contained about GrowReach.
- **Pricing stays in its section** — SaaS pricing in `pricing/`, lifetime deal pricing in `lifetime-deal/`. Don't merge them.

## Adding a new page

1. Create the `.mdx` file (with YAML frontmatter: `title` and `description`).
2. Add it to the navigation in `docs.json` — pages not listed in `docs.json` are deployed but hidden from the sidebar.
3. Push and verify the deploy on the [dashboard](https://app.mintlify.com).

## Previewing locally

Install the Mintlify CLI (`npm i -g mint`), then run `mint dev` from this directory — the preview serves at `http://localhost:3000`.
