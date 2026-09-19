NEXUS-X Ω Android V4 FIXED

Purpose:
VERIFY → ANALYZE → BACKTEST → AUDIT → RANK

This build fixes the V3 issues found during source review:
1. Track A textarea placeholder now renders real line breaks.
2. Seed/V3 migration normalizes prize tiers and prize weights.
3. Known footer artifact "2026" is excluded during normalization.
4. V3 browser data is migrated automatically into the V4 database when present.
5. Locked-cycle count counts only type=CYCLE locks, not Track-A-only locks or audits.
6. A+B locks store the training cutoff date and record count.
7. Result audit is tied to the latest immutable cycle and avoids duplicate audits.
8. Track A scoring exposes exact/family/rotation/reverse/9-Mirror/recent/gap/369/root/sum evidence.
9. PDF append keeps the QC gate and blocks duplicate draw dates.
10. Service-worker cache is version-bumped so the new code can replace stale V3 shell files.

Important:
- User candidates are temporary research input and are never inserted into the historical dataset.
- Scores are evidence summaries, not probabilities or guarantees.
- The app is browser-based and stores its research state locally in IndexedDB.
- First PDF parsing requires internet access to load PDF.js from CDN.

Deployment:
Upload the contents of this folder to the root of the GitHub Pages repository.
Then open the HTTPS Pages URL in Android Chrome.
If an older installed PWA still shows V3, close it fully and reopen the Pages URL; the V4 service worker has a new cache name and deletes the old nexus-x caches during activation.
