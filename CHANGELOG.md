# Release notes

## 0.21.0 — Desktop workflow upgrade

This release expands the Windows desktop workflow with task controls, code review, GitHub access and clearer verification evidence.

### Improvements

- Ask separately in a side conversation without changing the active task.
- Queue the next request or steer the current run, with persistent controls and paused recovery after Stop, failure or restart.
- Inspect task context, instruction sources, recorded file reads and estimated model input.
- Add line-level diff findings, resolve reviews and detect stale reviews after code changes.
- Connect through the installed GitHub CLI to browse repositories, clone projects, inspect branches, issues, pull requests and CI.
- Manage reader agents and isolated writer worktrees, preview integration and reject stale or conflicting snapshots.
- Mark image feedback and compare a local before-image.
- Test the configured endpoint/model with generation, tool, structured-output, vision and six-turn memory probes.
- Review delivery requirements, tests, visual evidence and outstanding blockers in one panel.

### Verification

647 automated tests and four packaged desktop suites passed. All 371 packaged first-party files matched the checked build. Installer executable, app archive and legal files match the tested package; private-path, credential-pattern and dependency-notice checks passed.

Desktop model and GitHub responses used controlled fixtures. Paid live-provider probes, live GitHub account actions and a clean Windows VM installation were not tested. Model probes are bounded checks, not a guarantee of long-task quality.

### Downloads and requirements

Use the installer or portable EXE. Close older CRIMINAL instances before upgrading. SHA256SUMS.txt covers the four accompanying files; the legal ZIP contains third-party notices and applicable covered sources. Windows x64 packages remain unsigned.

The GitHub dashboard needs Git, GitHub CLI and an account with repository access. Writer worktrees require Git. Side chat uses a task snapshot; queued requests currently accept text. Integration still requires relevant post-merge checks.

CRIMINAL is free for personal and commercial use under its Freeware License. Provider/API/cloud charges are separate. This repository contains public documentation and binary downloads; the application source and cloud-worker source kit are not published here.

## 0.14.7 — Browser verification, recovery and clearer summaries

- Added a GitHub project link in Settings for releases, feedback and updates.
- Fixed repeated verification loops caused by changing test timings, IDs, SQLite sidecars and generated QA files. Real project progress remains distinguishable from repeated checks.
- Improved recovery of corrected browser selectors and replacement owned servers, while retaining assertion, target, coverage and file-freshness checks.
- Browser requirements now use actual browser workflow evidence; API checks and window titles do not prove browser interactions. Successful browser assertions count as behavior verification.
- Improved delayed navigation checks and full-height visual capture beyond six screens, including dynamically growing pages. Incomplete capture remains reported.
- Made summaries clearer: current and historical failures are separated, successful browser journeys are visible, and raw stacks, long visual-review prose and helper files no longer crowd the result.
- Improved custom test-count parsing and Node warning-flag handling; syntax-only scripts do not count as behavior tests.

Validation: 517 automated tests and 10 packaged desktop suites passed. Portable self-extraction, native window and backend launch passed; 237 installer payload files matched the tested package. Tests used isolated provider fixtures. Live-provider quality and a clean-VM installation were not tested. Windows packages remain unsigned.

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


