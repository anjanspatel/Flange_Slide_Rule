# Anjan Patel — Engineering Tools

**Live → [tools.anjanpatel.ca](https://tools.anjanpatel.ca)** &nbsp;·&nbsp; **Repo → [github.com/anjanspatel/Tools](https://github.com/anjanspatel/Tools)**

A personal hub of precision engineering reference tools built for field and office use. Each tool is a self-contained, single-page app — no login, no tracking, no install.

---

## Tools

### [Flange Slide Rule](https://tools.anjanpatel.ca/flange/)

API 6A / ISO 10423 flange dimensional reference.

- Bore, OD, bolt pattern, and ring gasket data for all pressure ratings (3K – 15K)
- Covers 10 nominal sizes (1-13/16" through 11")
- Instant lookup — no typing, no tables to scroll
- PDF export with job/equipment note in the filename
- Imperial and metric display

---

### [Safety Block Calculator](https://tools.anjanpatel.ca/tubing/)

Safe working load for tubing blocks and safety blocks.

- Inputs: Brinell hardness (BHN), block width, and thickness
- Von Mises shear method — safety factor of 3
- 5-step breakdown showing every intermediate value
- Imperial / Metric toggle
- Print-to-PDF with watermark

---

## Stack

- **HTML / CSS / JS** — zero build step, zero dependencies
- **GitHub Pages** — deployed from `main`, custom domain via CNAME
- **Google Fonts** — IBM Plex Sans + IBM Plex Mono
- **jsPDF + html2canvas** — flange tool PDF export (inlined)
- **Canvas API** — animated background (aurora, beams, meteors, grid)

---

## Repo Structure

```
anjanspatel/Tools
/
├── index.html        ← Hub (landing page + tool cards)
├── CNAME             ← tools.anjanpatel.ca
├── favicon.svg
├── logo.png
├── flange/
│   └── index.html    ← Flange Slide Rule
├── tubing/
│   └── index.html    ← Safety Block Calculator
└── terms/
    └── index.html    ← Terms of Use & Disclaimer
```

Each tool is its own directory with a standalone `index.html`. To add a new tool: create a folder, add the page, link the card in `/index.html`.

---

## Legal

All tools are for **reference and informational purposes only**. Outputs must be verified by a licensed Professional Engineer before use.

Full terms: [tools.anjanpatel.ca/terms/](https://tools.anjanpatel.ca/terms/)

&copy; Anjan Patel. All rights reserved.
