---
layout: default
title: From Claude to Claude Code on Windows
description: Install Git for Windows and Claude Desktop, then open a safe local Code workspace on Windows 11.
---

<p class="eyebrow">Windows + Claude route | Part 1 of 2</p>

# From Claude to Claude Code on Windows

<div class="status-line">
  <span>Last checked: 27 July 2026</span>
  <span>Guide requires: updated Windows 11</span>
  <span>Extra requirement: Git for Windows</span>
</div>

<div class="assistant-note">
Guide the user through one numbered section at a time and wait for confirmation. Do not ask the user to open PowerShell, Command Prompt, Windows Terminal, Git Bash, or WSL. If a label differs from this page, ask the user to describe what they see rather than guessing. Use only the official Claude and Git for Windows download pages linked below.
</div>

Claude Code is the **Code** workspace inside Claude Desktop. It works directly on Windows without the command-line version or WSL. Local Code sessions do require Git for Windows, which Claude uses behind the scenes.

## 1. Check Windows and the processor type

1. Open **Start > Settings**.
2. Select **System > About**.
3. Under **Windows specifications**, confirm the edition is Windows 11.
4. Under **Device specifications**, find **System type**.
5. Confirm it says **64-bit operating system** and note whether the processor is **x64-based** or **ARM-based**.

Open **Settings > Windows Update** and install available system updates before continuing. Restart the PC if Windows requests it.

The processor type matters because Windows uses separate x64 and ARM64 installers. An Intel or AMD PC is normally x64. A Snapdragon-based PC is normally ARM64.

## 2. Make a folder for the first project

1. Open **File Explorer**.
2. Select **Documents** in the left sidebar.
3. Choose **New > Folder**.
4. Name the folder `Agent Projects`.
5. Open `Agent Projects` and create another new folder inside it.
6. Name the new folder `my-start-page`.

Claude Code will use `my-start-page` as its working directory. Manual mode asks before edits and commands, but the selected folder is not a hard filesystem sandbox. Reject any request to reach outside it unless you understand and approve the reason. For future projects, make and select a separate folder for each one.

## 3. Install Git for Windows

<a class="button" href="https://git-scm.com/download/win">Open the official Git for Windows download page</a>

1. Download the recommended 64-bit installer that matches the **System type** you noted: x64 or ARM64.
2. Open the downloaded setup file.
3. If Windows asks whether to allow the installer to make changes, continue only if you opened that prompt from the installer you just downloaded from `git-scm.com`. If Windows reports an unknown or unverified publisher, cancel and return to the official download page.
4. Keep the recommended installation options and complete the setup.
5. Close the installer. You do not need to open Git Bash or type a Git command.

Git is a tool Claude Code uses to manage project changes. Installing it does not require you to learn its command-line interface.

## 4. Install Claude Desktop

<a class="button" href="https://claude.com/download">Open the official Claude download page</a>

1. Choose the Windows download that matches your x64 or ARM64 system type.
2. Open the downloaded Claude setup file.
3. Follow the graphical installer and let it finish.
4. Open **Claude** from the Start menu.

The basic Code workspace does not require Windows virtualization or WSL. Do not enable those features for this guide.

## 5. Sign in and open Code

1. Sign in with the same Claude account as your subscription.
2. Complete any browser sign-in requested by the app.
3. Return to Claude Desktop and open **Code**.
4. If the app asks you to restart after sign-in or after finding Git, quit and reopen Claude.

If you see an upgrade message instead of Code, first check that the app is using the same account as your Claude subscription.

## 6. Open Claude Code in your safe folder

1. In **Code**, choose **Local**.
2. Select **Select folder**.
3. Choose **Documents > Agent Projects > my-start-page**.
4. Keep the permission mode on **Manual**.

Manual mode lets you review proposed file changes and commands before they happen. The selected folder is Claude's working directory, but you should still reject requests to reach outside it unless you understand why they are needed.

<div class="notice">
  <strong>Computer control is not needed.</strong>
  This first project does not require Claude to control other applications or see unrelated windows. Leave those optional features off if they are offered.
</div>

<div class="checkpoint">
  <strong>Checkpoint</strong>
  You should now see a Code conversation with <code>my-start-page</code> as its selected folder and the permission mode set to Manual. Do not paste the setup prompt into ordinary Claude Chat; paste it into Code.
</div>

<div class="next-step">
  <h2>Move into the local agent</h2>
  <p>The browser assistant has finished its part. The next page contains the shared handoff prompt.</p>
  <a class="button" href="../handoff/">Continue to the handoff</a>
</div>
