# Flange Slide Rule — API 6A

**Interactive quick-reference tool for API Specification 6A / ISO 10423 flange dimensions and pressure ratings.**

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-0B1F3A?style=flat-square&logo=github)](https://anjanspatel.github.io/Flange_Slide_Rule/)
[![Version](https://img.shields.io/badge/version-1.5-D97706?style=flat-square)](https://anjanspatel.github.io/Flange_Slide_Rule/)
[![License](https://img.shields.io/badge/license-Proprietary-667085?style=flat-square)](#license)

---

## Live Demo

**[https://anjanspatel.github.io/Flange_Slide_Rule/](https://anjanspatel.github.io/Flange_Slide_Rule/)**

No installation. No login. Works offline once loaded.

---

## Overview

The Flange Slide Rule is a standalone, single-file browser tool that replicates the experience of a physical slide rule for API 6A flanges. Select a nominal flange size and pressure rating directly on the engineering drawing, and all dimensions update instantly — bore, OD, raised face, hub, bolt circle, bolt count, stud diameter, stud length, ring gasket designation, and more.

Built for engineers and inspectors who need fast dimensional lookups in the field, in meetings, or on a rig — without pulling out a copy of API Spec 6A.

---

## Features

| Feature | Details |
|---|---|
| **Pressure ratings** | 3,000 · 5,000 psi |
| **Nominal sizes** | 2 1/16" · 2 9/16" · 3 1/8" · 4 1/16" · 5 1/8" · 7 1/16" · 9" · 11" · 13 5/8" · 16 3/4" |
| **Ring gaskets** | R and RX series (API 6B flanges) |
| **Unit toggle** | Inch (fractional + decimal) ↔ Metric (mm) — remembered across sessions |
| **Clipboard copy** | Click any dimension value to copy it to the clipboard |
| **PDF export** | One-page landscape PDF of the current configuration |
| **Dark / Light mode** | Toggle in the header — defaults to light, preference saved |
| **Offline ready** | Fully self-contained — works with no internet connection after first load |
| **Accessible** | Keyboard navigation, ARIA labels, skip link, visible focus states |
| **Responsive** | Scales on any screen size from mobile to widescreen |

---

## Dimensions Shown

For each size / rating combination the tool displays:

- **Bore** — nominal bore diameter
- **OD** — flange outside diameter
- **Raised Face (RF)** — raised face diameter
- **Hub OD** — hub outside diameter
- **Hub Min** — minimum hub length at bore
- **Bolt Circle (BC)** — bolt circle diameter
- **No. of Bolts** — number of stud bolts
- **Stud Bolt Dia.** — stud bolt diameter
- **Stud Length** — approximate stud length
- **Bolt Hole Dia.** — bolt hole diameter
- **Ring Gasket** — ring number (R-xx / RX-xx)
- **Corner Radius** — bore corner radius per rating

---

## How to Use

### Online
Open **[https://anjanspatel.github.io/Flange_Slide_Rule/](https://anjanspatel.github.io/Flange_Slide_Rule/)** in any modern browser.

### Offline / Local
1. Download `index.html` from this repository.
2. Open it directly in any browser — no server required.
3. All data and images are embedded; the file is fully self-contained.

### Usage
1. Use the **FLANGE SIZE** dropdown to select the nominal size.
2. Use the **PRESSURE RATING** dropdown to select 3,000 or 5,000 psi.
3. All dimensions update immediately on the engineering drawing.
4. Click any highlighted value to **copy** it to the clipboard.
5. Use **in / mm** to toggle between imperial and metric display.
6. Use **Download PDF** to export the current view as a one-page PDF.

---

## Technology

| | |
|---|---|
| **Architecture** | Single standalone HTML file — no build tools, no dependencies, no server |
| **Styling** | Vanilla CSS with CSS custom properties for theming |
| **Scripting** | Vanilla JavaScript (ES6+) |
| **Images** | Engineering drawing embedded as Base64 PNG — no external assets |
| **PDF export** | `html2canvas` + `jsPDF` (loaded from CDN on demand, only when PDF is requested) |
| **Persistence** | `localStorage` for theme and unit preferences only |
| **Hosting** | GitHub Pages (static, no backend) |

---

## Data Coverage

Data for **3,000 psi** and **5,000 psi** ratings across all 10 nominal sizes is based on API Specification 6A / ISO 10423 Table 6 (dimensional data) and Table 9 (ring gasket data), R and RX ring series.

> ⚠ Dimensions for nominal sizes **13 5/8"** and **16 3/4"** should be verified against the current controlled edition of API Spec 6A before engineering use.

---

## Engineering Disclaimer

This tool is a **quick-reference aid only**. It is not a substitute for the current controlled edition of API Specification 6A, manufacturer documentation, regulatory requirements, or project-specific engineering specifications.

All dimensions, pressure ratings, ring gasket designations, bolt data, and all other values must be **independently verified** before use in any engineering, design, fabrication, inspection, procurement, or recertification activity.

**Use at your own risk. No warranty is provided. See [Terms of Use](https://anjanspatel.github.io/Flange_Slide_Rule/) (footer of the live tool) for full terms.**

---

## Repository Structure

```
Flange_Slide_Rule/
├── index.html       # Complete standalone tool (all data, images, and logic embedded)
├── index.v1.3.html  # Archived — v1.3 with 10K/15K data, pre-accessibility update
└── README.md        # This file
```

---

## Versioning

| Version | Date | Notes |
|---|---|---|
| v1.0 | 2026-08 | Initial release — 3K/5K ratings, 8 sizes |
| v1.1 | 2026-08 | GitHub Pages deployment |
| v1.2 | 2026-08 | Published to main branch |
| v1.3 | 2026-08 | Added 10K/15K ratings, BX ring gaskets, 13 5/8" and 16 3/4" sizes, bolt hole display, metric toggle, clipboard copy, Terms & Privacy, favicon |
| v1.4 | 2026-08 | Print/PDF scale fix (222mm, 0.90 scale), accessibility (skip link, ARIA labels, focus states, modal focus trap, `<main>` landmark), watermark in PDF, job note first in filename |
| v1.5 | 2026-08 | Removed 10K/15K data — tool now covers verified 3K/5K data only; 13 5/8" and 16 3/4" retained |

---

## License

Copyright © 2026 Anjan Patel. All rights reserved.

This tool and all associated content, code, data, and design are the exclusive property of Anjan Patel. No part of this work may be reproduced, distributed, modified, or used to create derivative works without prior written permission.

See the Terms of Use and Privacy Policy in the footer of the live tool at [https://anjanspatel.github.io/Flange_Slide_Rule/](https://anjanspatel.github.io/Flange_Slide_Rule/).

---

## Contact

**Anjan Patel**
[LinkedIn](https://www.linkedin.com/in/anjanspatel/) · [anjan@anjanpatel.ca](mailto:anjan@anjanpatel.ca)
