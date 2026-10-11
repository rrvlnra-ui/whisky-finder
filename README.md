# Whisky Ratings Finder

Look up Scotch, Japanese and Australian whisky ratings by name or from a photo of the label, and keep your own tasting log. It runs as a web app you add to your iPhone Home Screen and Mac Dock.

## What's in the folder

| File | What it is |
|---|---|
| `index.html` | The app: rating sources, photo search, tasting log, rating-scale guide |
| `distilleries.js` | About 200 distilleries and brands, used to recognise labels and suggest names |
| `manifest.webmanifest` | App name and icons |
| `sw.js` | Lets the app open without a connection |
| `icons/` | App icons |

## Put it online (GitHub Pages)

Same steps as Onco Finder, in a new repository called `whisky-finder`:

1. On GitHub: **+ → New repository**, name `whisky-finder`, **Public**, **Create repository**.
2. Click **uploading an existing file**, drag in everything inside this folder (including `icons`), then **Commit changes**.
3. **Settings → Pages**: Branch **main**, folder **/ (root)**, **Save**.
4. After a minute or two it's at `https://<your-username>.github.io/whisky-finder/`.

## Install

- **iPhone:** open the address in Safari → **Share → Add to Home Screen**.
- **Mac:** open it in Safari → **File → Add to Dock**.

## Using it

- **Search by name:** type a bottle (for example *Lagavulin 16*) and press **Search**. Every source card then opens that search.
- **Search by photo:** tap **Photo**, take a straight-on picture of the front label in good light. The app reads the label on your device and matches it to its distillery list. Tap a different suggestion if it picked the wrong one, or edit the name. The first photo downloads the text reader, so it takes a little longer.
- **Open all:** opens the search on every source. Allow pop-ups for the site on Mac; on iPhone use **Open next**.
- **My tastings:** add a bottle with a photo, score out of 100 and notes. When you later search a bottle you've scored, the app shows your score.
- **Rating scales:** how each source scores, so a 90 from one can be compared sensibly with a 90 from another.

## Backups

Tastings and photos are stored on the device. Use **Export backup** on one device and **Import backup** on the other (AirDrop or iCloud Drive) to copy them across. Imports add to what's there and never overwrite.

## Updating

Upload changed files to the repository, and change `wf-v1` in `sw.js` to `wf-v2` (and so on) so installed copies refresh.
