# SocialExpand Webseite

Statische Webseite für socialexpand.com: eine Seite (`index.html`) mit Raketen-Intro, Referenz-Videos,
Glücksrad, Anfrage-Formular, Impressum und Login-Button (Team / Kunde → CRM).

- `index.html`: die ganze Seite, CSS und JavaScript stecken darin
- `videos/`: Referenz-Videos (H.264, 540 px breit) mit Vorschaubildern
- `fonts/`: Schriften lokal (Bricolage Grotesque, Onest, DM Mono), damit keine Daten an Google gehen
- `vercel.json`: Cache-Regeln für Videos und Schriften

## Hosting (Vercel)

1. Vercel → **Add New → Project** → dieses Repository wählen → **Deploy** (kein Build nötig).
2. Im Projekt **Settings → Domains** → `socialexpand.com` hinzufügen oder kaufen, `www.socialexpand.com` auf `socialexpand.com` weiterleiten.

Jeder Push auf `main` veröffentlicht die Seite neu.

## Login-Links

Der Login-Dialog verlinkt das CRM unter `socialexpand-crm.vercel.app`. Sobald dort `app.socialexpand.com` und
`kunden.socialexpand.com` verbunden sind (siehe README im CRM), werden die Links auf diese Adressen umgestellt.
