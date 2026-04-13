# images/

Alle Bilder die du hier reinlegst erscheinen automatisch in der Bilder-Sidebar des Editors und sind mit einem ★ markiert. Sie können nicht gelöscht werden (nur ausgeblendet nach Reload wenn du sie aus dem Ordner entfernst).

## Unterstützte Formate

`.png`, `.jpg`, `.jpeg`, `.gif`, `.webp`, `.svg`, `.bmp`

## Wie es funktioniert

Beim Laden der Seite versucht der Editor `images/manifest.json` zu laden. Diese Datei enthält einfach eine Liste aller Dateinamen.

### Automatisch (empfohlen)

Pusht du zu GitHub, baut der Workflow `manifest.json` automatisch aus dem Ordnerinhalt. Du musst nur Dateien reinwerfen und pushen.

### Manuell

Lokal vor dem Commit:

```bash
python build-manifest.py
```

Oder `manifest.json` von Hand anlegen:

```json
["logo.png", "hintergrund.jpg", "sprite.png"]
```

## Tipps

- **Pixel-Art:** Kleine Bilder (16×16, 32×32, 64×64) werden im Editor automatisch pixelperfekt skaliert
- **Dateinamen** ohne Leerzeichen und Sonderzeichen funktionieren am zuverlässigsten
- Keine Limit-Größe, aber bedenke: alles wird mit der Seite geladen
