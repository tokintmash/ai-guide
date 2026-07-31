---
layout: default
title: Set Up Claude Code in the Claude App on Windows
description: Install Git for Windows and the Claude desktop app, then open a local Claude Code session in its Code tab on Windows 11.
---

<p class="eyebrow">Windows + Claude route | Part 1 of 2</p>

# Set up Claude Code in the Claude app on Windows

<div class="status-line">
  <span>Last checked: 30 July 2026</span>
  <span>Guide requires: updated Windows 11</span>
  <span>Extra requirement: Git for Windows</span>
</div>

<div class="assistant-note">
Guide the user through one visible action at a time and wait for confirmation. Never ask the user to open PowerShell, Command Prompt, Windows Terminal, Git Bash, or WSL. If a label differs, ask what they see. Use only the official downloads linked below; stop for any other source. After the user confirms the section 5 checkpoint, tell them to stop using this setup conversation, switch to the Claude Code session in the Code tab of the Claude desktop app, and paste the next page's handoff prompt there. Then end your guidance; do not continue into the handoff or first project.
</div>

The installed app is named **Claude**. Its **Code** tab runs Claude Code directly in the desktop app. Claude Code is also available as a separate command-line interface, but this guide does not install or use that CLI. Local Windows sessions require Git for Windows, but not WSL.

## 1. Check Windows and the processor type

1. Open **Start**, then **Settings**.
2. Select **System**, then **About**.
3. Under **Windows specifications**, confirm the edition is Windows 11.
4. Under **Device specifications**, find **System type**.
5. Confirm it says **64-bit operating system** and note whether the processor is **x64-based** or **ARM-based**.

In Settings, select **Windows Update** and install available system updates before continuing. Restart the PC if Windows requests it.

Windows uses separate x64 and ARM64 installers, so use the type shown in About.

**You know it worked when:** About shows Windows 11 and either an x64-based or ARM-based processor.

## 2. Install Git for Windows

<a class="button" href="https://git-scm.com/download/win">Open the official Git for Windows download page</a>

1. Download the 64-bit Setup installer that matches the **System type** you noted: x64 or ARM64.
2. Open the downloaded setup file.
3. At a Windows security prompt, continue only for the installer from `git-scm.com`. Cancel if its publisher is unknown or unverified.
4. Complete the setup.
5. Close the installer. You do not need to open Git Bash or type a Git command.

Claude uses Git behind the scenes; you will not operate Git from a command line.

**You know it worked when:** the Git installation finishes without an error.

## 3. Install the Claude desktop app

<a class="button" href="https://claude.com/download">Open the official Claude download page</a>

1. For an x64-based PC, choose **Download for Windows**. For an ARM-based PC, choose **Windows (arm64)**.
2. Open the downloaded Claude setup file.
3. Follow the graphical installer and let it finish.
4. Open **Claude** from the Start menu.

The Code tab does not require Windows virtualization or WSL. Do not enable those features for this guide.

**You know it worked when:** Claude opens from the Start menu.

## 4. Sign in and open Code

1. Sign in with the same Claude account as your subscription.
2. Complete any browser sign-in requested by the app.
3. Return to the Claude desktop app and open the **Code** tab.
4. If the app asks you to restart after sign-in or after finding Git, select the **Show hidden icons** up arrow at the bottom-right of the taskbar. Otherwise, continue to the checkpoint below.
5. Then right-click the **Claude** icon and choose **Quit** or **Exit**. Closing only the window may leave Claude running in the background.
6. Open Claude again from the Start menu and return to the **Code** tab.

If you see an upgrade message instead of Code, first check that the app is using the same account as your Claude subscription.

**You know it worked when:** the **Code** tab opens in the Claude desktop app.

## 5. Start a Claude Code session and make the project folders

1. In the **Code** tab, choose **Local**.
2. Select **Select folder**.
3. In the folder window, select **Documents** in the sidebar. Windows may show it under **OneDrive** or **This PC**; select the Documents entry you see, not OneDrive or This PC itself. Do not type a location.
4. Use the folder window's control for creating a new folder. Name it `Agent Projects`, then open it.
5. Create another folder named `my-start-page`, then select only that folder.
6. Keep the permission mode on **Manual**.

`my-start-page` is Claude's working directory, not a hard filesystem sandbox. The **Code** tab has direct local-file access. **Manual** controls approvals, asking before edits and commands. Reject access outside the working directory unless you understand and approve it.

<div class="notice">
  <strong>Computer control is not needed.</strong>
  This first project does not require Claude to control other applications or see unrelated windows. Leave those optional features off if they are offered.
</div>

<div class="checkpoint">
  <strong>What success looks like</strong>
  You see a Claude Code session with <code>my-start-page</code> as its selected folder and <strong>Manual</strong> selected. Do not paste the setup prompt into the <strong>Chat</strong> tab; paste it into this session in the <strong>Code</strong> tab.
</div>

<div class="next-step">
  <h2>Switch to the Claude Code session</h2>
  <p>Stop using the setup-assistant conversation now; its role is finished. In the Claude desktop app, switch to the Claude Code session in the <strong>Code</strong> tab with <code>my-start-page</code> selected. The next page contains the prompt to paste there. Do not paste it into the <strong>Chat</strong> tab.</p>
  <a class="button" href="https://tokintmash.github.io/ai-guide/handoff/">Continue to the handoff</a>
</div>
