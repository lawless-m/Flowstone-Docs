# ShushYT

A tiny browser extension (built for Vivaldi, Manifest V3 style) that automatically mutes YouTube tabs until the actual video content starts playing — so you never hear another pre-roll ad. "No more loud ads!"

**Repo:** `~/Git/ShushYT`

Three files: `manifest.json`, `background.js` (tab mute/unmute logic and message handling), and `content.js` (the content script that watches the YouTube ad container DOM). Loads through `vivaldi://extensions` → "Load unpacked". The extension mutes every YouTube tab on load, monitors the ad container, and unmutes once the ad finishes. Sibling to [[DLPlug]] as the second browser extension in the corpus.
