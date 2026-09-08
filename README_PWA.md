# HM Trading Journal PWA V20

V20 fixes iPhone startup database popups and avoids compressed IndexedDB records that can fail to decode on Safari/iOS. Restore the original JSON backup once after installing V20; subsequent reloads use the uncompressed IndexedDB journal.

Upload `index.html`, `service-worker.js`, `manifest.json`, and `icons/` to the GitHub Pages root.
