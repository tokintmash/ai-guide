---
layout: default
title: From ChatGPT to Codex on Windows
description: Install the ChatGPT desktop app and open a safe native Codex workspace on Windows 11.
---

<p class="eyebrow">Windows + ChatGPT route | Part 1 of 2</p>

# From ChatGPT to Codex on Windows

<div class="status-line">
  <span>Last checked: 27 July 2026</span>
  <span>Guide requires: updated Windows 11</span>
  <span>Uses: ChatGPT desktop app</span>
</div>

<div class="assistant-note">
Guide the user through one numbered section at a time and wait for confirmation. Do not ask the user to open PowerShell, Command Prompt, Windows Terminal, or WSL. If a label differs from this page, ask the user to describe what they see rather than guessing. Stop if the download is not from <strong>chatgpt.com</strong>, <strong>openai.com</strong>, or the Microsoft Store.
</div>

Codex is part of the current ChatGPT desktop app. It runs natively on Windows; this route does not require WSL, a separate Codex program, or an API key.

## 1. Check Windows

1. Open **Start > Settings**.
2. Select **System > About**.
3. Under **Windows specifications**, confirm the edition is Windows 11.
4. Under **Device specifications**, find **System type**.
5. Confirm it says **64-bit operating system** and note whether the processor is **x64-based** or **ARM-based**.

Open **Settings > Windows Update** and install available system updates before continuing. Restart the PC if Windows requests it.

Codex also uses Microsoft's **App Installer** while preparing its stronger Windows sandbox:

1. Open **Settings > Apps > Installed apps** and search for `App Installer`.
2. If it is installed, open **Microsoft Store > Library > Get updates** so Windows can update it.
3. If it is missing, search for **App Installer** in Microsoft Store and install the version published by Microsoft Corporation.

You will not need to open or operate App Installer yourself after that.

This beginner route targets Windows 11. Although parts of Codex can run on recent Windows 10 versions, OpenAI describes that support as best effort, and ordinary Windows 10 is no longer a suitable baseline for the current Node.js setup.

## 2. Make a folder for the first project

1. Open **File Explorer**.
2. Select **Documents** in the left sidebar.
3. Choose **New > Folder**.
4. Name the folder `Agent Projects`.
5. Open `Agent Projects` and create another new folder inside it.
6. Name the new folder `my-start-page`.

Codex will receive access to `my-start-page`, not the whole Documents folder or even the parent `Agent Projects` folder. For future projects, make and select a separate folder for each one.

## 3. Install the official app

<a class="button" href="https://chatgpt.com/download/">Open the official ChatGPT download page</a>

1. Choose the Windows download.
2. Allow the official Microsoft installer or Store page to open.
3. Select **Install** or **Get** and wait for it to finish.
4. Open **ChatGPT** from the Start menu.

Use the current ChatGPT app that includes Codex. Do not install an unofficial app or a product described as ChatGPT Classic.

## 4. Sign in

1. Select **Continue to sign in**.
2. Complete sign-in in the browser window that opens.
3. Use the same ChatGPT account as your subscription.
4. Return to the desktop app when the browser finishes.

Do not choose API-key authentication. API keys use separate billing and are not needed for this guide.

## 5. Open Codex in your safe folder

1. Open **Codex** in the ChatGPT desktop app.
2. Choose **Add new project** or the option to open a local folder.
3. Select **Documents > Agent Projects > my-start-page**.
4. Keep the permission setting on **Ask for approval**.
5. If Codex offers to prepare its recommended Windows sandbox, review the explanation and approve the Windows security prompt.

The sandbox setup may require an administrator confirmation. Approve it only when it was opened by the official ChatGPT app. Do not right-click ChatGPT and run the whole app as Administrator.

**Ask for approval does not mean Codex asks before every file change.** It can normally create and edit files and run routine PowerShell commands inside the selected folder. It asks before actions such as using the network or reaching outside that folder. Selecting one empty project folder keeps that automatic access narrow.

<div class="notice">
  <strong>Computer control is not needed.</strong>
  This first project does not require Codex to control other applications or see the rest of your screen. Leave those optional features off if they are offered.
</div>

<div class="checkpoint">
  <strong>Checkpoint</strong>
  You should now see a new Codex conversation with <code>my-start-page</code> as its local folder. Do not paste the setup prompt into ordinary ChatGPT chat; paste it into this Codex conversation.
</div>

<div class="next-step">
  <h2>Move into the local agent</h2>
  <p>The browser assistant has finished its part. The next page contains the shared handoff prompt.</p>
  <a class="button" href="../handoff/">Continue to the handoff</a>
</div>
