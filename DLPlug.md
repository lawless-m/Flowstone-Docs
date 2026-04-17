# DLPlug

A Chrome/Edge [[BrowserExtension]] (Manifest V3) that streams web videos to VLC via yt-dlp — click the extension icon on any page with a video and the backend native-messaging host pipes the yt-dlp-extracted URL straight into a running VLC, bypassing the browser's built-in player entirely.

**Repo:** `~/Git/DLPlug`

Three pieces. A Chrome extension with a `background.js` service worker and the `nativeMessaging` and `activeTab` permissions — manifest name "DLPlug", description "Stream videos to VLC via yt-dlp". A `host/` folder containing the native messaging host that receives URLs from the extension and spawns `yt-dlp` piped into `vlc`. An `install.sh` that registers the native host with Chrome. The whole thing is small enough that the manifest plus the install script are effectively the spec — no README needed.
