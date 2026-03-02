# hekaton.berlin — Site Maintenance

**Live:** https://hekaton.netlify.app
**Repo:** https://github.com/prometheus2211/hekaton-site (privat)
**Deploy:** automatisch via Netlify bei jedem Push auf `main`

---

## Neue Cowork-Session starten

Kopiere das Folgende am Anfang eines neuen Cowork-Chats:

```
Hekaton-Site Maintenance.

GitHub Repo: https://github.com/prometheus2211/hekaton-site.git
GitHub Token: [neuen Token generieren unter github.com/settings/tokens]
Live-URL: https://hekaton.netlify.app
Lokaler Pfad: /mnt/1 - Corporate Identity/Website/hekaton-site/

Workflow für Updates:
1. Datei bearbeiten: hekaton-site/index.html
2. git add . && git commit -m "Beschreibung" && git push
3. Netlify deployed automatisch (~30 Sek)

Aktuelle Version: hekaton-v16.html (Backup im CI-Ordner)
Logo-Datei: hekaton-site/logo.png (Hekaton-Logo-White-300dpi.png)
index.html ist ~26KB — Logo ist extern, nicht als Base64 eingebettet.
```

---

## Token abgelaufen?

1. github.com → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token → Scope: `repo` → Token kopieren
3. Im Repo-Ordner: `git remote set-url origin https://NEUER-TOKEN@github.com/prometheus2211/hekaton-site.git`

---

## Netlify Forms

- Formular-Name: `hekaton-vorstellung`
- Einreichungen: Netlify Dashboard → Forms
- E-Mail-Benachrichtigungen: Forms → hekaton-vorstellung → Form notifications
- Kontakt-E-Mail: contact@hekaton.berlin

---

## Häufige Änderungen — wo suchen in index.html

| Was                   | HTML-Anker                 |
|-----------------------|----------------------------|
| Eyebrow (Prometheus)  | `<p class="h-eye">`        |
| Hero-Headline         | `<h1 class="h-hl">`        |
| Claim (dark section)  | `<div id="break">`         |
| Statistiken           | `<section id="success">`   |
| Phasen + Fördergelder | `<section id="phases">`    |
| Formular-Fragen       | `<section id="introduce">` |
| Impressum / Datenschutz | `<div class="modal-bg">`  |
| Footer                | `<footer>`                 |

Alle Texte haben `data-d` (Deutsch) und `data-e` (Englisch) — immer beide anpassen.

---

## Fördergelder (Stand März 2026)

- Ideation: Mentoring & Co-Creation
- Incubation: bis zu 15.000 €
- Acceleration: bis zu 50.000 €
