# Pixel Studio

Ein 16:9 Bild-Editor direkt im Browser. Erstelle Designs mit Text, Formen und Bildern – alles mit scharfem Pixel-Rendering und Minecraft-Style Fonts.

**[➜ Live Demo](#)** _(Link nach Deployment eintragen)_

## Features

- 🎨 16:9 Canvas mit anpassbarer Hintergrundfarbe
- 🖼️ Bilder hochladen und mit Drag & Drop platzieren
- 🔤 Fonts hochladen (.ttf, .otf, .woff, .woff2)
- ✏️ Text-Werkzeug mit eingebauten Pixel-Fonts (Press Start 2P, Jersey 10, Pixelify Sans, VT323, Silkscreen)
- 📐 Formen: Rechteck, Kreis, Dreieck, Linie
- 🔄 Rotation, Flipping, Opacity, Layer
- ↩️ Undo/Redo (bis zu 60 Schritte)
- 📋 Rechtsklick-Menü mit Duplizieren, Kopieren, Sperren etc.
- 🎯 Snap-Guides beim Verschieben
- 💾 Export als scharfes PNG (720p, 1080p, 4K oder native)
- ⚡ Pixel-Art Rendering ohne Blur (nearest-neighbor)

## Nutzung

Nichts zu installieren – einfach die Live-Demo öffnen.

### Tastenkürzel

| Shortcut | Aktion |
|---|---|
| `Strg+Z` / `Strg+Y` | Rückgängig / Wiederholen |
| `Strg+D` | Duplizieren |
| `Strg+C` / `Strg+V` | Kopieren / Einfügen |
| `Entf` | Objekt löschen |
| `Pfeiltasten` | Objekt verschieben (Shift = 10px) |
| `Scroll` | Objekt skalieren |
| `Doppelklick` auf Text | Text bearbeiten |
| `Shift` beim Drehen | In 15°-Schritten rasten |
| `Rechtsklick` | Kontextmenü |

## Hinweis zur Speicherung

Diese GitHub-Version speichert **nichts** auf einem Server. Alles läuft im Browser:

- Hochgeladene Bilder und Fonts existieren nur in deiner aktuellen Session
- Beim Reload der Seite sind sie weg
- Deine Designs verlassen deinen Computer nie

Das Endergebnis speicherst du ganz normal als PNG über den Export-Button.

## Deployment auf GitHub Pages

1. Dieses Repo forken oder erstellen
2. `index.html` ins Root-Verzeichnis
3. In den Repo-Settings: **Pages** → Branch `main` / Folder `/ (root)` auswählen
4. Deine Seite ist unter `https://<username>.github.io/<repo>/` erreichbar

Alternativ per GitHub Action (siehe `.github/workflows/pages.yml`).

## Lokale Entwicklung

Da alles statisch ist, reicht ein beliebiger kleiner HTTP-Server:

```bash
python -m http.server 8080
# oder
npx serve .
```

Dann `http://localhost:8080` im Browser öffnen.

## Lizenz

MIT
