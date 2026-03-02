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
2. git add index.html && git commit -m "Beschreibung" && git push
3. Netlify deployed automatisch (~30 Sek)

Backup-Versionen: /1 - Corporate Identity/Website/hekaton-v1.html bis hekaton-v13.html
Aktuelle Version: hekaton-v13.html
Logo (Dark Nav): /1 - Corporate Identity/Logos/Hekaton-Logo-White-300dpi.png
Logo (Light BG): /1 - Corporate Identity/Logos/Hekaton-Logo-CMYK-300dpi.png
```

---

## Token abgelaufen?

1. github.com → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token → Scope: `repo` → Token kopieren
3. Dann Claude mitteilen: neuer Token ist `ghp_...`

---

## Netlify Forms

- Formular-Name: `hekaton-vorstellung`
- Einreichungen ansehen: Netlify Dashboard → Forms
- E-Mail-Benachrichtigungen: Forms → hekaton-vorstellung → Form notifications

---

## Häufige Änderungen — wo suchen in index.html

| Was                  | HTML-Anker              |
|----------------------|-------------------------|
| Hero-Headline        | `<h1 class="h-hl">`     |
| Claim (dark section) | `<div id="break">`      |
| Statistiken          | `<section id="success">`|
| Phasen-Texte         | `<section id="phases">` |
| Formular-Fragen      | `<section id="introduce">`|
| Footer               | `<footer>`              |

Alle Texte haben `data-d` (Deutsch) und `data-e` (Englisch) Attribute — immer beide anpassen.
