# DayPlan (Mein Tagesplan)

Tagesplaner als Web-App für das iPhone: Ernährung, Gym, Uni (mit Lern-Drache) und Gebet.

## Dateien

- `index.html` – die ganze App (HTML, CSS und JavaScript in einer Datei)
- `manifest.webmanifest` – Name und Symbole für den Home-Bildschirm
- `sw.js` – Service Worker, damit die App auch ohne Internet startet
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` – App-Symbole

Die Daten werden nur lokal im Browser deines iPhones gespeichert (localStorage).

## Kostenlos online stellen

Die App muss einmal unter einer https-Adresse erreichbar sein. Danach läuft sie auf dem iPhone ohne Mac.

### Variante A: Netlify (am einfachsten)

1. Gehe auf https://app.netlify.com/drop und melde dich kostenlos an.
2. Ziehe den ganzen Ordner `DayPlan` in das Feld.
3. Netlify gibt dir eine Adresse wie `https://irgendein-name.netlify.app`.

### Variante B: GitHub Pages

1. Erstelle bei https://github.com ein neues Repository, zum Beispiel `dayplan`.
2. Lade alle Dateien aus diesem Ordner hoch.
3. Öffne im Repository **Settings → Pages**, wähle den Branch `main` und den Ordner `/ (root)`.
4. Nach ein bis zwei Minuten ist die App unter `https://DEINNAME.github.io/dayplan/` erreichbar.

## Auf dem iPhone installieren

1. Öffne die Adresse **in Safari**.
2. Tippe auf **Teilen** (Quadrat mit Pfeil) → **Zum Home-Bildschirm** → **Hinzufügen**.
3. Starte die App künftig immer über das Symbol auf dem Home-Bildschirm.

## Hinweise

- Die Daten aus der Vorschau-Version (claude.ai) werden nicht übernommen, du fängst neu an.
- Die Daten liegen nur auf diesem iPhone. Wenn du die Safari-Websitedaten löschst oder die App vom Home-Bildschirm entfernst, sind sie weg.
- Nach einer Änderung an den Dateien neu hochladen. Die App holt sich beim nächsten Start mit Internet die neue Version. Wenn nötig, erhöhe `V` in `sw.js` (zum Beispiel `dayplan-v2`).
- Die Gebetszeiten werden im Gerät berechnet. Wähle im Gebet-Tab deine Stadt, Standard ist Siegen.
