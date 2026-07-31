---
layout: default
title: Install Node.js on Mac
description: Install Node.js LTS on a Mac with the official graphical package installer.
---

<p class="eyebrow">Mac | Only when the local agent says Node is missing</p>

# Install Node.js on Mac

Node.js lets the agent run the small local web project in this guide. Use the official Mac package installer; do not use Homebrew, a version manager, or a pasted installation command.

<div class="status-line">
  <span>Last checked: 27 July 2026</span>
  <span>Choose: LTS</span>
  <span>File type: macOS Installer (.pkg)</span>
</div>

## 1. Download the installer

<a class="button" href="https://nodejs.org/en/download">Open the official Node.js download page</a>

1. Make sure the page shows **LTS**, not **Current**.
2. Choose macOS if the page has not detected it automatically.
3. Download the **macOS Installer (.pkg)**.

The official package works on supported Intel and Apple Silicon Macs. You do not need to choose a processor type for the `.pkg` installer.

## 2. Run the Mac installer

1. Open **Finder > Downloads**.
2. Double-click the downloaded file ending in `.pkg`.
3. Follow the Installer steps and leave the standard components selected.
4. When macOS asks for administrator approval, use the Mac's normal password or Touch ID in the system dialog.
5. Close the Installer when it reports success.

<div class="notice">
  <strong>Keep the password out of chat.</strong>
  A password request from the macOS Installer window is normal for this system-wide installation. Type it only into that Mac dialog. The AI does not need to see it.
</div>

## 3. Return to the desktop agent

Return to the same Codex chat in the ChatGPT desktop app or Claude Code session in the **Code** tab of the Claude desktop app. Do not send this message to the old setup conversation. Paste:

```text
The official Node.js macOS package installer finished successfully. Please check `node --version` and `npm --version` again. Do not install or upgrade anything else. When both checks pass, resume the Agentic Desktop Starter Guide where we left off and lead me into the first project; do not wait for me to provide another command.
```

If the agent still cannot find Node:

1. Quit the ChatGPT or Claude desktop app completely.
2. Open it again from Applications.
3. Return to the same Codex chat or Claude Code session.
4. Ask it to repeat the two checks.

Restarting the app allows it to see software that was installed after the app opened.

<div class="checkpoint">
  <strong>Checkpoint</strong>
  The agent should now report a Node version beginning with <code>v</code> and an npm version number. You do not need to run or type either command yourself.
</div>

<div class="next-step">
  <h2>Node is ready</h2>
  <p>The local agent should now ask what title you want and continue leading the project.</p>
  <a class="button" href="https://tokintmash.github.io/ai-guide/first-project/">Follow along with the first project</a>
</div>
