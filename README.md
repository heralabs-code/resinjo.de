# ReSinJo (German site)

Source for **www.resinjo.de** – statische Onepager-Website für die Marke ReSinJo (HERATEC Export u. Beteiligungsges. mbH).

Reines HTML/CSS/vanilla JS, kein Build-Schritt, kein Framework. `index.html` direkt im Browser öffnen für eine lokale Vorschau.

- Design-Spec: siehe [resinjo.com](https://github.com/heralabs-code/resinjo.com), Datei `docs/superpowers/specs/2026-09-11-resinjo-onepager-design.md` (gemeinsame Spec für beide Seiten)
- Englische Schwester-Seite: [resinjo.com](https://github.com/heralabs-code/resinjo.com) → www.resinjo.com

## Struktur

- `index.html` – die Onepager-Seite
- `impressum.html` – Impressum
- `datenschutz.html` – Datenschutzhinweise
- `styles.css`, `script.js` – gemeinsames Styling/Verhalten (Mobil-Navigation)
- `assets/` – Platzhalter-Favicon; `logo-placeholder.svg` ist nur eine Referenzkopie (wird von keiner Seite eingebunden)
- `sitemap.xml`, `robots.txt`, `CNAME` – Hosting-/SEO-Konfiguration für GitHub Pages

## Bekannte Platzhalter

Suche nach `PLATZHALTER` in `index.html` und `impressum.html` — die Kommentare markieren das noch einzusetzende endgültige Logo.

**Vor dem Live-Gang:** Datenschutzhinweise anhand des tatsächlichen Betriebs prüfen: Bei STRATO gilt die AVV laut Anbieter für Verträge ab 18.07.2022 automatisch; ältere Verträge müssen im Kundenkonto geprüft werden. Klären, welche Datenschutzvereinbarung GitHub Pages tatsächlich abdeckt, Drittlandübermittlungen bewerten und die interne Aufbewahrung von Anfragen festlegen. Laut Betreiber gibt es derzeit keinen bestellten Datenschutzbeauftragten. Die Händlerlinks führen auf eigenständige Shops.

## Änderungen veröffentlichen

Diese Seite hat keinen Build-Schritt. Für die Veröffentlichung auf GitHub Pages müssen der Pages-Dienst aktiviert und die DNS-Einträge der Domain auf GitHub Pages gerichtet sein. Die Datei `CNAME` benennt nur die gewünschte Domain und konfiguriert DNS nicht selbst.

**Prüfstand 24.09.2026:** `www.resinjo.de` zeigt per DNS auf STRATO und leitet über HTTP zu `heratec.de` weiter; HTTPS auf `www.resinjo.de` schlägt fehl. `https://heralabs-code.github.io/resinjo.de/` liefert 404. Die Dateien dieses Repos sind daher unter der ReSinJo-Domain derzeit nicht veröffentlicht. Ein Commit auf `main` allein ändert das nicht.
