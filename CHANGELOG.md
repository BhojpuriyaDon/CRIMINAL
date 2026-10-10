# Release notes

## 0.22.0 — Direct provider presets

Connect directly to supported AI provider APIs; OpenRouter remains optional.

- Added 34 endpoint presets across hosted APIs, regional/deployment endpoints and local servers. Protocol variants and regions count separately; this is not a count of distinct vendors.
- Presets configure endpoints, protocols, authentication guidance and official setup links. Saved profiles stay separate, unsaved key/model drafts clear on preset changes, and stale connection checks cannot overwrite the active selection.
- Added manual model/deployment entry where discovery differs, including Azure. Custom provider profiles remain available.
- Direct API formats include OpenAI Chat Completions, OpenAI Responses, Anthropic Messages and Gemini. Other vendor-specific signing or OAuth flows need a compatible gateway.

### Verification

685 automated tests passed, including 38 provider tests. The packaged provider desktop suite and portable launch/provider/icon checks passed. Tests used fixtures; paid live-provider calls and a clean Windows VM installation were not tested. Windows x64 packages remain unsigned.

### Downloads and limits

The installer, portable EXE, third-party legal bundle, license and SHA256 checksums are attached to [release v0.22.0](https://github.com/BhojpuriyaDon/CRIMINAL/releases/tag/v0.22.0). Provider access and model capabilities depend on the user's account. This release does not publish application or cloud-worker source.

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
