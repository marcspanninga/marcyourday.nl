# marcyourday.nl

Coming soon pagina voor **Marc Your Day**, gebouwd met HTML, Tailwind CSS (v4) en Alpine.js.

## Lokaal werken

```bash
npm install
npm run dev     # Tailwind in watch-modus, schrijft naar assets/css/site.css
```

Open daarna `index.html` via een lokale server, bijvoorbeeld `python3 -m http.server`.

## Publiceren

Elke push naar `main` bouwt de CSS (`npm run build`) en publiceert de site via GitHub Pages
(`.github/workflows/pages.yml`). `assets/css/` wordt niet gecommit; die bouwt de workflow.

## Bestanden

- `index.html`: de pagina; Alpine regelt de lopende tijdcode en de pauzeknop voor beweging
- `src/input.css`: Tailwind-bron met de huisstijlkleuren en lettertypen
- `assets/img/logo.svg`: logo voor donkere achtergrond (crème tekst, gouden hoeken)
- `assets/img/logo-dark.svg`: logo voor lichte achtergrond
- `assets/img/logo-currentcolor.svg`: logo waarvan de tekst de tekstkleur overneemt
- `assets/img/favicon.svg`: icoon voor het browsertabblad

De letters in de logo's zijn omgezet naar paden (Cormorant Garamond Medium), dus ze zien er overal hetzelfde uit, ook zonder het lettertype.
