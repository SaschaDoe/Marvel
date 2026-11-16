# Marvel Zeitlinien-Atlas

Interaktive Karte aller Marvel-Filme und -Serien (MCU, Sony, Fox und frühe Filme). Figuren, Gegenspieler, Artefakte und Handlungsstränge laufen als Fäden durch die Titel, in denen sie vorkommen.

Inoffizielle Fan-Seite ohne Verbindung zu Marvel, Disney oder Sony. Die Seite enthält Spoiler.

## Aufbau

| Pfad | Inhalt |
| --- | --- |
| `index.html` | Die komplette Seite: Daten, Layout und Logik in einer Datei |
| `img/` | Fotos von Wikimedia Commons (Darsteller, Cosplay, Nachbauten) |
| `netlify.toml` | Einstellungen für Netlify, kein Build-Schritt |

Es gibt keine Abhängigkeiten und keinen Build. Lokal ansehen:

```bash
python -m http.server 8000
```

Danach `http://localhost:8000` öffnen.

## Auf Netlify veröffentlichen

1. Bei Netlify anmelden und **Add new site → Import an existing project** wählen.
2. GitHub verbinden und dieses Repository auswählen.
3. Build command leer lassen, Publish directory `.` (steht schon in `netlify.toml`).
4. **Deploy** klicken. Jeder weitere Push auf `main` veröffentlicht automatisch neu.

## Inhalte pflegen

Alle Daten stehen im `<script>`-Block von `index.html`:

- `TT`: Titel (Kennung, Reihe, Datum, Name, Marke, Inhalt)
- `HH`: Fäden (Kennung, Typ, Name, Beschreibung, Stationen mit Notiz)
- `LOOKS`: Erscheinungen je Faden mit Foto, Bildnachweis und Suchbegriff für Filmbilder

## Bilder und Rechte

Die Seite enthält keine Filmszenen und kein offizielles Artwork. Die Fotos in `img/` stammen von Wikimedia Commons und stehen unter freien Lizenzen (überwiegend CC BY und CC BY-SA). Urheber, Lizenz und Quelle jedes Fotos stehen auf der Seite unter „Bildnachweise“ und in `LOOKS`. Wer die Fotos weiterverwendet, muss diese Angaben übernehmen.

Die Links „Filmbilder“ öffnen eine Bildersuche außerhalb der Seite.

Marvel, die Figuren- und Filmtitel sind Marken ihrer jeweiligen Inhaber.
