# Levi45 IPTV Converter v3.3

Static GitHub Pages playlist editor and converter.

## Classic Quick Converter

A two-textbox conversion interface has been added beneath the channel library. Paste M3U text, select an output format, click Convert Playlist, inspect or edit the output, and download it. For Enigma2 choose Download Userbouquet (.tv). The Download M3U File button saves the displayed text with an .m3u extension and is intended for M3U output.

## Deploy

Copy `index.html`, `css/style.css`, and `js/script.js` to your existing repository in the same folders. The tool runs entirely in the browser.

Existing channel editing, drag sorting, autosave, project backup and restore remain available.


## v3.3.2 fix
Initialises `restoring`, `saveTimer`, and `PROJECT_KEY` before autosave runs.


## v3.4 additions
Selected-channel Enigma2 preview (first 300 channels for responsiveness), copy preview, and separate full M3U and Enigma2 download buttons. Category grouping continues to use `group-title` metadata; channels without a category appear as Uncategorised. Preview edits are not used for downloads; use the channel editor to change channel data.
