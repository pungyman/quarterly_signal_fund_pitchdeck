# Quarterly Signal Fund Pitch Deck

Pitch deck materials for the Quarterly Signal Fund. The repo includes two Slidev decks (Markdown) and a standalone HTML deck.

## Setup

Install dependencies once:

```bash
npm install
```

## Main pitch deck (Slidev)

Serves `slides.md`:

```bash
npm run dev
```

Open **http://localhost:3030/** in your browser.

**Navigation:** arrow keys / Space (next), Shift+arrow (previous), `o` (overview), `f` (fullscreen).

## Wealth Management variant (Slidev)

Serves `wm_slides.md` (7 / 13 / 16 / 20 stock portfolio variants):

```bash
npx slidev wm_slides.md
```

Slidev picks another port if 3030 is already in use (often 3031).

## Standalone HTML deck

`index.html` is a self-contained deck (alphaBT / Quarterly Equity Strategy Engine). Open it directly:

```bash
open index.html
```

Or serve it locally:

```bash
python3 -m http.server 8080
```

Then open **http://localhost:8080/index.html**.

**Navigation:** arrow keys, Space, scroll wheel, or the ‹ › buttons at the bottom.

## Quick reference

| Deck | File | Command |
|------|------|---------|
| Main pitch | `slides.md` | `npm run dev` → http://localhost:3030 |
| WM portfolios | `wm_slides.md` | `npx slidev wm_slides.md` |
| HTML deck | `index.html` | `open index.html` or static server |

## Other scripts

```bash
npm run build   # build Slidev deck for production
npm run export  # export slides (e.g. PDF)
```
