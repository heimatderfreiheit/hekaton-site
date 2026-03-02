# hekaton.berlin

Landing page — single-file, self-contained HTML.

## Deployment (Netlify via GitHub)

1. Diesen Ordner (`hekaton-site/`) als GitHub Repo hochladen
2. netlify.com → "Add new site" → "Import an existing project" → GitHub verbinden
3. Build settings: leer lassen (kein Build nötig)
4. Deploy — fertig

## Domain

Netlify → Domain settings → `hekaton.berlin` hinzufügen
Beim Domain-Provider: CNAME `www` → `[dein-site-name].netlify.app`

## Formular

Einreichungen erscheinen automatisch unter:
Netlify → Forms → `hekaton-vorstellung`
Dort E-Mail-Benachrichtigungen aktivieren.

## Änderungen

Datei `index.html` editieren → Git commit → push → Netlify deployt automatisch.
