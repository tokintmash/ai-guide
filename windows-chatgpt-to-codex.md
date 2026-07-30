---
layout: default
title: From ChatGPT to Codex on Windows
description: Install the ChatGPT desktop app and open a safe native Codex workspace on Windows 11.
---

<p class="eyebrow">Windows + ChatGPT route | Part 1 of 2</p>

# From ChatGPT to Codex on Windows

<div class="status-line">
  <span>Last checked: 29 July 2026</span>
  <span>Guide requires: Windows 11</span>
  <span>Uses: ChatGPT desktop app</span>
</div>

<div class="assistant-note">
Guide the user through one numbered section at a time and wait for confirmation. Do not ask the user to open PowerShell, Command Prompt, Windows Terminal, or WSL. If a label differs from this page, ask the user to describe what they see rather than guessing. Use only the official download button below. It may open the Microsoft Store or OpenAI's documented, Store-signed installer from <strong>get.microsoft.com</strong>; stop for any other download source.
</div>

Codex is part of the current ChatGPT desktop app. It runs natively on Windows; this route does not require WSL, a separate Codex program, or an API key.

## 1. Check Windows

1. Open **Start**, select **Settings**, then select **System** and **About**.
2. Under **Windows specifications**, confirm that the edition is Windows 11.

**You know it worked when:** the About page shows Windows 11.

This beginner route targets Windows 11. OpenAI describes Windows 10 support as best effort; see [troubleshooting](https://tokintmash.github.io/ai-guide/troubleshooting/) if this PC has Windows 10.

## 2. Install the official app

<a class="button" href="https://chatgpt.com/download/">Open the official ChatGPT download page</a>

1. Choose the Windows download.
2. Allow the official Microsoft installer or Store page to open.
3. Select **Install** or **Get** and wait for it to finish.
4. Open **ChatGPT** from the Start menu.

Use the current ChatGPT app that includes Codex. The same download page also offers **ChatGPT Classic**, which does not include this Codex workspace; do not choose Classic or an unofficial app.

**You know it worked when:** ChatGPT opens from the Start menu.

## 3. Sign in

1. Select **Continue to sign in**.
2. Complete sign-in in the browser window that opens.
3. Use the same ChatGPT account as your subscription.
4. Return to the desktop app when the browser finishes.

Do not choose API-key authentication. API keys use separate billing and are not needed for this guide.

**You know it worked when:** the desktop app returns from the browser and its profile menu shows the account you signed into.

## 4. Open Codex and make the project folder

1. Open **Codex** in the ChatGPT desktop app.
2. Choose **Add new project** or the option to open a local folder.
3. In the folder window, select **Documents** in the sidebar. Windows may show Documents under **OneDrive** or **This PC**; use the Documents entry you see and do not type a location.
4. Use the folder window's **New folder** control to make a folder named `Agent Projects`, then open it.
5. Make another new folder named `my-start-page`, then select that folder.
6. Keep the permission setting on **Ask for approval**.
7. If Codex offers to prepare its recommended Windows sandbox, review the explanation and approve the Windows security prompt.

The sandbox setup may require an administrator confirmation. Approve it only when it was opened by the official ChatGPT app. Do not right-click ChatGPT and run the whole app as Administrator.

Folder-name capitalization does not matter on ordinary Windows folders, so `Agent projects` and `Agent Projects` refer to the same folder.

**The working folder is a safety boundary, not just a filing choice.** In this sandboxed setup, Codex blocks filesystem writes outside the working folder and asks before network access. It can create and edit files inside `my-start-page` without asking before each change. Keep **Ask for approval**, do not attach more folders, and do not switch to full access. A separate folder for each future project keeps this writable area narrow.

<div class="notice">
  <strong>Computer control is not needed.</strong>
  This first project does not require Codex to control other applications or see the rest of your screen. Leave those optional features off if they are offered.
</div>

<div class="checkpoint">
  <strong>Checkpoint</strong>
  You know it worked when you see a new Codex conversation with <code>my-start-page</code> as its local folder and <strong>Ask for approval</strong> selected. Do not paste the setup prompt into ordinary ChatGPT chat; paste it into this Codex conversation.
</div>

<div class="next-step">
  <h2>Move into the local agent</h2>
  <p>The browser assistant has finished its part. The next page contains the shared handoff prompt.</p>
  <a class="button" href="https://tokintmash.github.io/ai-guide/handoff/">Continue to the handoff</a>
</div>
