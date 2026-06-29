# Arbeitsweise fuer dieses Repository

Hinweise fuer Claude Code und andere Agenten, die in diesem Repo arbeiten.

## Was das hier ist

Oeffentliche Lernressourcen (statisches HTML/CSS), veroeffentlicht ueber
GitHub Pages aus dem Root des `main`-Branches. Es gibt keinen Build-Schritt:
Was im Repo liegt, ist genau das, was ausgeliefert wird.

## Branching und Deploy

- **Kein Feature-Branch noetig.** Direkt auf `main` arbeiten, committen und
  nach `main` pushen.
- **Deploy passiert automatisch.** Jeder Push auf `main` loest den Workflow
  "pages build and deployment" aus und veroeffentlicht die Aenderungen ohne
  weiteres Zutun.
- **Kein Pull Request noetig**, ausser der Mensch bittet ausdruecklich darum.
- Inhalte sind oeffentlich lesbar; keine privaten Daten committen.

## Struktur und Konventionen

- Jeder Kurs liegt in einem eigenen Ordner (z. B. `spotify-mixing/`) mit:
  - `index.html` als Kursuebersicht
  - `lessons/NNNN-*.html` fuer Lektionen (vierstellig nummeriert)
  - `reference/NNNN-*.html` fuer druckbare Referenzen
  - `assets/` fuer CSS, Bilder und SVGs (gemeinsames `course.css`)
  - `MISSION.md`, `RESOURCES.md`, `NOTES.md` als Workspace-Dateien
- Sprache der Inhalte: Deutsch. Im Code werden Umlaute umschrieben
  (ae, oe, ue) statt echter Umlaute.
- Quellen im Text verlinken; inhaltliche Aussagen belegbar halten.
- Auf Mobil und Druck achten (`course.css` enthaelt bereits `@media print`
  und Scroll-Wrapper fuer Tabellen).
