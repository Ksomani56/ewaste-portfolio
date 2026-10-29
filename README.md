# Krishna Somani · E-Waste Management Portfolio

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Site-orange?style=flat&logo=github)](https://ksomani56.github.io/ewaste-portfolio/)
[![License](https://img.shields.io/badge/License-Academic-blue.svg)](#license)

An interactive, visual portfolio archiving coursework, case studies, datasets, and infographics produced for the **E-Waste Management** course under the **Department of Computer Engineering, Vellore Institute of Technology (VIT)**.

🌐 **Live Website:** [https://ksomani56.github.io/ewaste-portfolio/](https://ksomani56.github.io/ewaste-portfolio/)

---

## 📌 Table of Contents

- [Overview](#overview)
- [Key Portfolio Artifacts](#key-portfolio-artifacts)
- [Project Architecture](#project-architecture)
- [Running Locally](#running-locally)
- [Adding New Assignments](#adding-new-assignments)
- [Safe File Note](#safe-file-note)
- [Author & Credits](#author--credits)

---

## Overview

This static web application features:
- **Uttar Pradesh State E-Waste Dashboard**: Interactive tracking of generation vs. collection across 6 key industrial districts (Lucknow, Kanpur, Ghaziabad, Gautam Buddh Nagar, Varanasi, Agra).
- **100-Point State Scorecard**: Audited scores across 7 key compliance categories (Generation, Collection, Formal Recycling, Regulatory Compliance, Informal Sector Integration, Environmental & Health Safeguards, Awareness).
- **Interactive Periodic Elements Viewer**: 3D-flippable element cards detailing critical recoverable materials (Ta, Nb, Ga, Pd, Rare Earths).
- **Coursework Archive**: Direct access to case studies, analytical workbooks, and high-resolution infographics.

---

## Key Portfolio Artifacts

| Artifact | Format | Description | Action |
| :--- | :--- | :--- | :--- |
| **E-Waste Comparison Overview** | Image (`.jpg`) | Handwritten country comparison: 2015 vs. 2019, CAGR, and collection rates | In-browser modal viewer |
| **State E-Waste Tracker** | PDF (`.pdf`) | Detailed Uttar Pradesh case study across 6 districts and 7 categories (72/100 Good Band) | Opens in new tab |
| **Tracker Workbook** | Excel (`.xlsx`) | 7-sheet auditable dataset & scorecard formulas behind the UP study | Direct download |
| **Carbon Footprint Task** | Excel (`.xlsx`) | Carbon accounting calculations, offsets, and emissions data (Jan–Aug 2026) | Direct download |
| **PCB Sorting Techniques** | Image (`.jpeg`) | Infographic: Combinatory sorting and isolation of tantalum, niobium, gallium, palladium | In-browser modal viewer |
| **E-Waste Activity Map** | Image (`.png`) | Kerala district-level e-waste production and recycling rates (2025) | In-browser modal viewer |

*Upcoming coursework topics (*Heavy Metals Risks*, *Indian Companies Compliance*, *Maharashtra E-Waste Paradox*, *Laser-Assisted Recovery*, *LEED v5 Green Building Score Studio*, and *10 E-Waste Case Studies*) will be published as they are completed.*

---

## Project Architecture

The project has zero build dependencies (pure HTML5, CSS3, vanilla JavaScript, and Canvas):

```text
ewaste-portfolio/
│
├── index.html                       # Core portfolio application (layout, interactive canvases, data)
├── README.md                        # Documentation & project information
└── files/                           # Static assets & assignment deliverables
    ├── carbon-footprint.xlsx        # Carbon footprint workbook
    ├── country-comparison.jpg       # Handwritten comparison infographic
    ├── elements-infographic.jpeg    # Critical raw materials PCB sorting
    ├── kerala-infographic.png       # Kerala generation & recycling map
    ├── state-ewaste-tracker.xlsx    # UP 7-sheet scorecard dataset
    └── up-case-study.pdf            # UP e-waste management study report
```

---

## Running Locally

Since this site uses standard web APIs and relative asset links, you can preview it with any static HTTP server:

```bash
# Clone the repository
git clone https://github.com/Ksomani56/ewaste-portfolio.git
cd ewaste-portfolio

# Start a local HTTP server using Python:
python -m http.server 8000

# Open in browser:
# http://localhost:8000
```

---

## Adding New Assignments

When ready to link a previously pending card to its file:

1. Copy the target file (`.pdf`, `.png`, `.jpg`, or `.xlsx`) into the `files/` folder.
2. In `index.html`, locate the `ITEMS` array:
   - Change that item's `k` property from `"none"` to `"img"`, `"pdf"`, or `"xls"`.
   - Add the path `u: "files/<filename>"`.
3. Commit and push the changes:
   ```bash
   git add files/ index.html
   git commit -m "Add deliverable: <item title>"
   git push origin main
   ```

---

## Safe File Note

All downloadable spreadsheets (`.xlsx`) and PDFs (`.pdf`) in this repository are clean academic deliverables created for educational purposes. They contain standard data tables, formulas, and charts with **no macros, VBA scripts, or executable code**. 

If your browser flags the download, it is due to default browser heuristics on newly hosted domains serving spreadsheet files; selecting **"Keep"** will open the file normally.

---

## Author & Credits

- **Author:** Krishna Somani
- **Roll Number:** 24102C0067
- **Department:** Computer Engineering
- **Institution:** Vellore Institute of Technology (VIT)
