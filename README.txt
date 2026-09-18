NEXUS-X Ω Android V3 — Fully Browser-Based

No Python server is required by the application itself.

1. Host this folder on an HTTPS web host.
2. Open index.html through that HTTPS URL in Android Chrome.
3. Upload Kerala State Lottery result PDFs directly in the app.
4. The PDF is parsed in the browser using PDF.js.
5. QC must PASS before the permanent dataset is updated.
6. Track A and Track B are isolated; locks are stored in IndexedDB.
7. Result audits and exports stay in the browser.

PDF.js is loaded from the official Mozilla project distribution via CDN.
The first load needs internet access; after the app shell is cached, the core UI/data can remain available offline. PDF parsing library availability can still depend on browser cache/network.

Research disclaimer: outputs are statistical evidence summaries, not winning guarantees or probabilities.
