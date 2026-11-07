DAILY EXPENSE MANAGER V4
========================
Files:
- index.html
- manifest.webmanifest
- service-worker.js
- icon-192.png
- icon-512.png

PUBLISHING
Upload ALL files into the ROOT of your GitHub Pages repository.
GitHub Pages -> Settings -> Pages -> Deploy from branch -> main -> /(root).
Open the published HTTPS URL in Safari, allow it to load, then Share -> Add to Home Screen.

SECURITY
- Uses Web Crypto PBKDF2 (310,000 iterations) and AES-GCM 256-bit encryption.
- Expense records and receipt photos are encrypted before being written to IndexedDB.
- Passphrase cannot be reset. Forgetting it means losing access to the vault.
- Lock screen is a local privacy barrier, not server-side authentication.
- Keep iPhone passcode enabled and export encrypted backups regularly.
- Never share your passphrase or backup file.
- Clearing Safari website data can delete the local vault.

OCR / OFFLINE LIMITATION
This build loads Tesseract.js from jsDelivr when the OCR feature is used. The app shell and saved expenses are offline-capable after the first visit, but the OCR engine itself is NOT bundled in this package. For reliable offline OCR, OCR engine, worker, WebAssembly core, and language model files must be bundled on the same origin and cached before going offline. Connect to the internet to use OCR. English printed text only; verify every suggested amount before saving.

DATA
All expense records remain in this browser's local IndexedDB. No sync/server account is included.
