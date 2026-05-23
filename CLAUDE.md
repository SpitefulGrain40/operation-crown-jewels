# Operation Crown Jewels — GitHub Pages Deployment

## What This Is
A complete set of printable HTML files and a prep tracker for a children's all-day escape room / murder mystery, built for Agent Nyxie (age 7). All files are fully self-contained HTML — no build step, no npm, no dependencies beyond Google Fonts CDN.

## Your Job
Deploy this project to GitHub Pages so the owner can access all printables and the tracker from any device at a stable URL.

## Steps

### 1. Check for an existing repo
Ask the user if they already have a GitHub repo for this. If not, create one called `operation-crown-jewels`.

### 2. Initialise and push
```bash
cd /path/to/site/folder
git init
git add .
git commit -m "Deploy Operation Crown Jewels — full mission pack"
git branch -M main
git remote add origin https://github.com/USERNAME/operation-crown-jewels.git
git push -u origin main
```

### 3. Enable GitHub Pages
```bash
gh repo edit --enable-pages --pages-branch main --pages-path /
```
Or via GitHub UI: Settings → Pages → Source: main branch → / (root) → Save.

### 4. Confirm URL
`https://USERNAME.github.io/operation-crown-jewels/`

---

## Complete File Index

| File | Description | Pages |
|------|-------------|-------|
| `index.html` | Mission Hub — links to everything | — |
| `00_mission_prep_tracker.html` | Interactive prep checklist with localStorage | — |
| `01_opening_letter.html` | Opening letter from Commander Crownsworth | 1 |
| `02_envelope.html` | Decorative envelope (superseded by labels) | — |
| `03_detective_dossier.html` | Dossier cover, rank tracker, badge log | 3 |
| `04_envelope_labels.html` | 9 RDA address labels for clue envelopes | 1 |
| `05_act1_playroom.html` | Crime scene notice, drawer labels, scrambled sentence | 3 |
| `06_act2_garage.html` | Geraferty's witness statement (climbing wall) | 1 |
| `07_act3_garden.html` | Lamby's note + garden evidence sheet | 2 |
| `08_act4_chickencoop.html` | Daddy Ooo Ooo's letter with 5 mistakes | 1 |
| `09_act5_gymnastics.html` | Four Star of the Week gymnastics vault + cipher | 1 |
| `10_acts6_7_8.html` | Balcony lookout, office suspect report, final trail cards | 3 |
| `11_culprit_reveal.html` | Confession letter from all four stuffies | 1 |
| `12_certificate_and_menu.html` | Royal Detective First Class certificate + tea menu | 2 |

## Notes
- All files are static HTML — GitHub Pages serves them perfectly.
- The tracker uses localStorage — works on GitHub Pages (not on file://).
- Google Fonts loaded via CDN — needs internet for correct fonts when viewing.
- Do NOT rename files — index.html links to them by filename.
