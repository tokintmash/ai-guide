---
layout: default
title: Install Node.js on Windows
description: Install Node.js LTS on Windows 11 with the official graphical MSI installer.
---

<p class="eyebrow">Windows | Only when the local agent says Node is missing</p>

# Install Node.js on Windows

Node.js lets the agent run the small local web project in this guide. Use the official Windows installer; do not use winget, Chocolatey, a version manager, PowerShell, or a pasted installation command.

<div class="status-line">
  <span>Last checked: 27 July 2026</span>
  <span>Choose: LTS</span>
  <span>File type: Windows Installer (.msi)</span>
</div>

## 1. Confirm the processor type

1. Open **Start > Settings > System > About**.
2. Under **Device specifications**, find **System type**.
3. Note whether it says **x64-based processor** or **ARM-based processor**.

Use x64 for an Intel or AMD PC. Use ARM64 for an ARM-based PC such as a Snapdragon PC. Always make the decision from **System type**, not the computer's marketing name. The current Node.js installer does not support 32-bit Windows.

## 2. Download the installer

<a class="button" href="https://nodejs.org/en/download">Open the official Node.js download page</a>

1. Make sure the page shows **LTS**, not **Current**.
2. Choose **Windows** if the page has not detected it automatically.
3. Choose x64 or ARM64 to match **System type**.
4. Download the **Windows Installer (.msi)**.

## 3. Run the Windows installer

1. Open **File Explorer > Downloads**.
2. Double-click the downloaded file ending in `.msi`.
3. Follow the setup steps and keep the standard Node.js, npm, and PATH options selected.
4. If the installer offers to install tools for native modules, leave that optional box unchecked. Those large developer tools are not needed for this project.
5. When Windows asks whether to allow the installer to make changes, confirm it is the Node.js installer you just downloaded and select **Yes**.
6. Finish and close the installer. A Windows restart is not normally required.

<div class="notice">
  <strong>Keep administrator credentials out of chat.</strong>
  A Windows User Account Control prompt is normal for this system-wide installation. Approve it yourself or enter an administrator password only in the Windows security dialog. The AI does not need to see it.
</div>

## 4. Return to the desktop agent

Return to the same Codex chat in the ChatGPT desktop app or Claude Code session in the **Code** tab of the Claude desktop app. Do not send this message to the old setup conversation. Paste:

```text
The official Node.js Windows MSI installer finished successfully. Please check `node --version` and `npm.cmd --version` again. Do not install or upgrade anything else. When both checks pass, resume the Agentic Desktop Starter Guide where we left off and lead me into the first project; do not wait for me to provide another command.
```

If the agent still cannot find Node:

1. At the bottom-right of the Windows taskbar, select the **Show hidden icons** up arrow. If there is no arrow, look for the app icon directly in that area.
2. Right-click the **ChatGPT** or **Claude** icon and choose **Quit** or **Exit**. Closing only the app window is not enough because the app may still be running in the background.
3. Open the app again from the Start menu.
4. Return to the same Codex chat or Claude Code session.
5. Ask it to repeat the two checks.

Fully quitting the app allows it to see the PATH update made by the installer. Opening only a new chat or session, or closing only the app window, may not be enough.

If you cannot find the app's notification-area icon or a **Quit** or **Exit** option, restart the computer. Then reopen the app, return to the same Codex chat or Claude Code session, and ask the agent to repeat the checks.

<div class="checkpoint">
  <strong>Checkpoint</strong>
  The agent should now report a Node version beginning with <code>v</code> and an npm version number. You do not need to run or type either command yourself.
</div>

<div class="next-step">
  <h2>Node is ready</h2>
  <p>The local agent should now ask what title you want and continue leading the project.</p>
  <a class="button" href="https://tokintmash.github.io/ai-guide/first-project/">Follow along with the first project</a>
</div>
