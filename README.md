# Meilenweit Voraus – VSL Landing Page

## Setup (2 Schritte)

### 1. Meta Pixel ID einsetzen
Öffne `index.html` und ersetze **beide** Vorkommen von `DEINE_PIXEL_ID` mit eurer echten Facebook Pixel ID.

```
Suchen:   DEINE_PIXEL_ID
Ersetzen: 123456789012345
```

### 2. Deployen

**Option A – Netlify Drag & Drop**
1. netlify.com → "Add new site" → "Deploy manually"
2. Den gesamten `mwv-vsl-deploy` Ordner reinziehen
3. Fertig ✓

**Option B – Netlify via GitHub**
1. Dieses Repo auf GitHub pushen
2. Netlify → "Import from Git" → Repo auswählen
3. Build command: leer lassen
4. Publish directory: `.`
5. Deploy ✓

**Option C – GitHub Pages**
1. Repo Settings → Pages → Branch: `main` → Folder: `/ (root)`
2. URL: `https://[username].github.io/[repo-name]`

## Custom Domain
Netlify: Domain settings → `training.meilenweitvoraus.com` → CNAME auf Netlify-URL setzen

## Testmodus
URL mit `?preview=1` öffnen → CTA wird nach 1,2 Sek. freigeschaltet (für Tests)

## Pixel Events
| Event | Trigger |
|-------|---------|
| `PageView` | Seite geladen |
| `Lead` | CTA nach 16 Min. freigeschaltet |
| `InitiateCheckout` | Klick auf "Jetzt Kurs sichern" |

## Video
Das Video läuft direkt via Vimeo MP4. Falls die URL abläuft:
Zeile mit `const VIMEO_URL` in index.html aktualisieren.
