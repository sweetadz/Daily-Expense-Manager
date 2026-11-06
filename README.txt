DAILY EXPENSE MANAGER V3 — PKR

Included: index.html, manifest, service worker, icons. Features: manual expense entry, receipt photo attachment, today/month totals, monthly budget, category report, month/category filters, delete, CSV export, full JSON backup and restore. Data is stored in IndexedDB on the device/browser.

IPHONE INSTALL / OFFLINE:
1. Upload all files in this folder to a static HTTPS website you control, keeping them together.
2. Open the HTTPS address in Safari while online and allow the app to finish loading once.
3. Safari Share -> Add to Home Screen -> Add.
4. Launch from the Home Screen icon. After first successful online load, the app shell is cached and can open offline. Entries remain local to that browser/device.
5. Use Backup regularly.

IMPORTANT: A service worker cannot install from a file:// URL or a file opened directly in the Files app. HTTPS hosting and one initial online visit are required for PWA offline launch. Receipt photo is stored locally, but OCR/automatic total reading is not included; enter the receipt total manually. Clearing Safari website data may erase local records. JSON restore merges records by ID.
