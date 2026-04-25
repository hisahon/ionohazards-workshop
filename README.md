# IonoHazards Workshop

**Workshop on Ionospheric Disturbances from Natural Hazards**  
*Official website repository — hosted via GitHub Pages*

---

## About

This repository contains the source code for the public website of the **IonoHazards** workshop series — a scientific meeting on ionospheric disturbances associated with natural hazards and extreme events, bringing together researchers from seismology, ionospheric physics, atmospheric science and space weather.

The workshop is associated with the **IONO-DIET** project (*Ionospheric Detection and Imaging of Earthquakes and Tsunamis in Near-Real-Time*, FAPESP process 22/03502-6), a collaboration between INPE (Brazil) and IPGP (France).

---

## Live Site

🌐 **[hisahon.github.io/ionohazards-workshop](https://hisahon.github.io/ionohazards-workshop)**

---

## Repository Structure

```
ionohazards/
│
├── index.html          ← Root redirect — always points to the current edition
│
├── 2026/
│   └── index.html      ← First edition · INPE, São José dos Campos · Oct 19–21, 2026
│
└── README.md
```

Each year's edition is archived in its own subdirectory. Old URLs remain permanently accessible. The root `index.html` always redirects visitors to the most recent edition.

---

## Editions

| Year | Dates | Venue | Status |
|------|-------|-------|--------|
| [2026](./2026/) | 19–21 October 2026 | INPE — São José dos Campos, SP, Brazil | **Upcoming** |

---

## Adding a New Edition

When organising a new edition:

1. Create a new directory: `mkdir 2027`
2. Copy and update the previous edition: `cp 2026/index.html 2027/index.html`
3. Edit dates, speakers and schedule inside `2027/index.html`
4. Update `index.html` at the root to redirect to `2027/`
5. Commit and push — the site updates automatically

```bash
git add .
git commit -m "Add 2027 edition"
git push
```

---

## Local Development

No build tools required. Open directly in a browser:

```bash
# Option 1 — open the file directly
open 2026/index.html

# Option 2 — serve locally (avoids any path issues)
python3 -m http.server 8000
# then visit http://localhost:8000/2026/
```

---

## Technical Notes

- Pure HTML/CSS — no JavaScript frameworks, no build step, no dependencies
- All fonts loaded from Google Fonts (Newsreader + JetBrains Mono)
- Fully static — works on any web host, not just GitHub Pages
- No cookies, no analytics, no tracking

---

## Institutions

| Acronym | Institution | Country |
|---------|-------------|---------|
| INPE | Instituto Nacional de Pesquisas Espaciais | Brazil |
| IPGP | Institut de Physique du Globe de Paris | France |
| USP | Universidade de São Paulo | Brazil |
| UnB | Universidade de Brasília | Brazil |
| Univap | Universidade do Vale do Paraíba | Brazil |
| IGP | Instituto Geofísico del Perú | Peru |
| CSN | Centro Sismológico Nacional, U. de Chile | Chile |

---

## Funding

This workshop is supported by **FAPESP** — Fundação de Amparo à Pesquisa do Estado de São Paulo.

---

*© IonoHazards Workshop Committee · MMXXVI*
