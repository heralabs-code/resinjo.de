# ReSinJo (German site)

Source for **www.resinjo.de** – statische Onepager-Website für die Marke ReSinJo (HERATEC Export u. Beteiligungsges. mbH).

Reines HTML/CSS/vanilla JS, kein Build-Schritt, kein Framework. `index.html` direkt im Browser öffnen für eine lokale Vorschau.

- Design-Spec: siehe [resinjo.com](https://github.com/heralabs-code/resinjo.com), Datei `docs/superpowers/specs/2026-09-11-resinjo-onepager-design.md` (gemeinsame Spec für beide Seiten)
- Englische Schwester-Seite: [resinjo.com](https://github.com/heralabs-code/resinjo.com) → www.resinjo.com

## Struktur

- `index.html` – die Onepager-Seite
- `impressum.html` – Impressum
- `styles.css`, `script.js` – gemeinsames Styling/Verhalten (Mobil-Navigation)
- `assets/` – Platzhalter-Favicon; `logo-placeholder.svg` ist nur eine Referenzkopie (wird von keiner Seite eingebunden)
- `sitemap.xml`, `robots.txt`, `CNAME` – Hosting-/SEO-Konfiguration für GitHub Pages

## Bekannte Platzhalter

Suche nach `PLATZHALTER` in `index.html` und `impressum.html` — Kontaktdaten und Impressum-Pflichtangaben müssen noch ergänzt werden. Das findet auch die `PLATZHALTER: ...`-Kommentare (Kommentar mit dem Hinweis auf das einzusetzende Logo), die markieren, wo das echte Logo eingesetzt werden muss – es ist direkt im HTML eingebunden, an 2 Stellen pro Datei, keine austauschbare Asset-Datei.

**Vor dem Live-Gang:** außerdem den kursiven Hinweis am Anfang von `impressum.html` entfernen ("Diese Seite ist ein Entwurf und keine Rechtsberatung..."). Das ist normaler Fließtext, kein `PLATZHALTER`-Marker, wird von der Suche oben also nicht gefunden.

## Änderungen veröffentlichen

Diese Seite hat keinen Build-Schritt – GitHub Pages liefert die Dateien in diesem Repo genau so aus, wie sie committet sind. Um eine Änderung zu veröffentlichen: Datei bearbeiten (direkt auf github.com oder wie auch immer gewünscht), auf den Branch `main` committen – nach etwa einer Minute ist die Änderung live unter www.resinjo.de. Die Datei `CNAME` nicht löschen oder umbenennen – die sagt GitHub, unter welcher Domain diese Seite läuft.
