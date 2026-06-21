# Kaia Selects – Website

Statische Website, gehostet über **GitHub Pages**. Premium-Geschenkboxen aus Südafrika.

## Dateien
- `index.html` – Landing Page (Warteliste via Tally)
- `corporate.html` – Firmenkunden (Anfrage via mailto an info@kaiaselects.de)
- `impressum.html` – Impressum
- `datenschutz.html` – Datenschutzerklärung
- `sitemap.xml` / `robots.txt` – SEO
- `og-image.jpg` – Social-Vorschaubild (1200×630)
- `CNAME` – verbindet die Domain mit GitHub Pages (Inhalt: `www.kaiaselects.de`)

## Setup
- **Domain:** kaiaselects.de (registriert bei IONOS, DNS zeigt auf GitHub Pages)
- **Warteliste:** Tally (tally.so/r/81RjyY)
- **E-Mail:** info@kaiaselects.de (Weiterleitung)
- **Monitoring:** Google Search Console

## Wenn die Seite nicht erreichbar ist
1. **Browser-/DNS-Cache:** Hard Refresh (Strg+F5 / Cmd+Shift+R) oder Inkognito-Fenster testen.
2. **GitHub Pages live?** Erst die `*.github.io`-Adresse direkt aufrufen. Lädt die → Problem liegt an der Domain/DNS, nicht am Inhalt.
3. **Domain führt auf „Hi there"/Platzhalter:** Meist fehlt die `CNAME`-Datei im Repo. Sie wird bei manchen Deploys versehentlich entfernt → neu anlegen mit Inhalt `www.kaiaselects.de` und in den Repo-Settings unter „Pages → Custom domain" erneut setzen.
4. **DNS prüfen:** IONOS-Records müssen auf GitHub Pages zeigen (A-Records auf GitHub-IPs + CNAME für www).
5. **Status:** githubstatus.com prüfen, ob GitHub Pages selbst eine Störung hat.

## Wichtig
- Dateinamen exakt kleingeschrieben halten (`corporate.html` etc.) – interne Links und Sitemap hängen daran.
- Bei Änderungen `CNAME` nie löschen, sonst trennt sich die Domain.
