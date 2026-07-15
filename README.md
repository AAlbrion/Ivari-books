# Ivari-books

Bücher (PDF) für **Ivaris World**, ausgeliefert über das jsDelivr-CDN.

## So lädst du ein Buch hoch

1. Lege die **rohe PDF** in den Ordner [`raw/`](raw/) (GitHub → „Add file" → „Upload files").
2. Ein GitHub Action komprimiert sie **automatisch** mit Ghostscript (`/ebook`, 150 dpi
   — Bilder bleiben erhalten, nur die Datei wird kleiner) und legt das fertige PDF
   in [`books/`](books/) ab. Wird die Datei durch die Komprimierung nicht kleiner,
   bleibt automatisch das Original erhalten.
3. Die App liest das Buch über die jsDelivr-URL:

   ```
   https://cdn.jsdelivr.net/gh/AAlbrion/Ivari-books@main/books/DATEINAME.pdf
   ```

> Nach dem Upload dauert die Komprimierung ein paar Minuten (Tab „Actions").
> jsDelivr-Links können nach einer Änderung bis zu ~24 h gecacht sein — für eine
> sofortige Aktualisierung notfalls einen neuen Dateinamen verwenden.

## Ordner

- `raw/`   — deine Original-PDFs (Quelle)
- `books/` — automatisch komprimierte, ausgelieferte PDFs (nicht von Hand bearbeiten)
