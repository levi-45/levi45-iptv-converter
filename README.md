# Levi45 IPTV Converter v3.0

A redesigned, static, privacy-friendly IPTV playlist converter. No backend, dependencies, or build step required.

## Run
Open `index.html` in a modern browser, or upload `index.html`, `style.css`, and `app.js` to the root of your GitHub Pages repository.

## Features
- Import M3U/M3U8/TXT by drag-and-drop, file picker, or paste
- Parse `#EXTINF` metadata, group titles, and common streaming URL schemes
- Preview, search, group-filter, select, and deselect channels (100 per page)
- Optional deduplication by identical stream URL and A–Z sorting
- Export Enigma2 bouquets with selectable service types 4097, 5001, 5002, 8193, or 1
- Grouped Enigma2 bouquets in a ZIP with a `bouquets.tv` snippet
- Export extended M3U, simple M3U, or plain URL lists
- Dark/light themes, responsive layout, and entirely local processing

## Enigma2 installation
Back up `/etc/enigma2/` before editing. Upload `userbouquet.*.tv` files there and append the provided `bouquets.tv.snippet.txt` entries to the existing `bouquets.tv` (do not overwrite it). Restart the Enigma2 GUI. Service type compatibility depends on your receiver's installed playback plugins.

## Notes
- Enigma2 service reference URL escaping follows common IPTV bouquet conventions; receiver implementations vary. Test on your target image and player.
- This converter does not fetch stream URLs or test whether streams are live. Only use playlists and streams you have permission to access.
- Some HLS master playlists are stream manifests rather than channel lists; they are not expanded.
- Very large playlists can use significant browser memory.
- Grouped ZIP uses uncompressed ZIP entries for portability and offline operation.

## v3.1 Playlist creator and editor

Use **Add channel** to create a list from scratch. Use **Edit** to change channel names, stream URLs, group/category, TVG ID and logo. Use **Add group** to start a new category, **Remove selected** to delete channels, and **Move up/down** to reorder one selected channel (disable alphabetical sorting first). Export the edited list as M3U or Enigma2. Changes remain in browser memory until export; save your file before leaving or refreshing. GitHub Pages needs only these four static files in the repository root.
