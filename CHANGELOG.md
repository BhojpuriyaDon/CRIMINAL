# Release notes

## 0.14.6 — Recovery, document checks and delivery fixes

- Recognizes narrowly verified recovery of corrected local JavaScript artifact-generation failures across document, spreadsheet, image, data and code tasks. Unchanged assertions and current file evidence are required; unrelated successful checks do not clear failures.
- Improves recognition of meaningful Node and saved PowerShell verification scripts, and recovery of read-only process/window probes.
- Checks Office/PDF content with extracted text and supports exact slide, sheet and page counts. Office owner-lock metadata no longer invalidates file checks; malformed PDF shells are rejected.
- Streams presence and hash checks for large output files without claiming their content or playback has been verified.
- Final summaries include actual script-created deliverables from the current request, filter helper/render-cache files, and summarize unresolved errors in clearer language.
- Restores eligible document, image and media files under artifacts/ to preview discovery.
- Retries malformed visual-review JSON once with the same images and remaining budget. Repeated malformed responses remain inconclusive.
- Updates bundled document, presentation, spreadsheet and PDF workflow guidance.

Validation: 507 automated tests, 8 packaged desktop suites, portable launch checks and 237 installer payload file comparisons passed. Provider fixtures were controlled; live provider behavior and a clean-VM installer run were not tested. Windows packages remain unsigned.

## 0.14.5 — Conversation, visual review and delivery fixes

- Visual review streams all targets in two-image batches, removing the old 12-target and 60-image task cutoffs while preserving budget, cancellation and coverage checks.
- Fallback answers lead with primary deliverables such as Blender projects and videos, keep helper files in Activity, and preserve real verification gaps.
- A failed read-only executable lookup can recover from a later successful absolute-path version check of the same executable. PATH requirements and unrelated failures stay protected.
- Includes the 0.14.4 conversation intent fix.

### Conversation intent fix (0.14.4, included in 0.14.5)

- Questions such as “tumhe kisne develop kiya hai” and “tumhe kis company ne build kiya hai” now receive direct answers in Project Work mode instead of false missing-file warnings and repair loops.
- Questions referring to filenames no longer seed file-creation acceptance requirements. Separate explicit implementation requests still require real work.
- System instructions distinguish the CRIMINAL publisher from the selected model developer and API provider.
- Regression coverage includes consecutive questions in native and compatibility modes, real build completion guards, and the packaged desktop chat.

## 0.14.3 — Free public Windows release

- Free personal, educational and commercial use under the CRIMINAL Freeware License, published by BhojpuriyaDon.
- A new **Settings → License** panel makes the EULA, third-party notices and covered-source information readable offline.
- **Open license folder** provides access to the full notice bundle, Electron/Chromium notices and MPL component source archives.
- Installer displays the license. Installer and portable packages carry the same license documents and third-party sources.
- Original CRIMINAL source remains private; public release assets contain the Windows app and required legal materials.

This release retains the 0.14.2 completion reports, per-request changed-file summaries, diff preview and guarded text Undo.

The Windows packages are unsigned. AI providers, web services and cloud compute may charge separately. No provider credits are included.
