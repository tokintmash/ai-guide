---
layout: default
title: From ChatGPT to Codex
description: Install the ChatGPT desktop app and open a safe local Codex workspace on a Mac.
---

<p class="eyebrow">ChatGPT route | Part 1 of 2</p>

# From ChatGPT to Codex

<div class="status-line">
  <span>Last checked: 26 July 2026</span>
  <span>Requires: macOS 14 or later</span>
  <span>Uses: ChatGPT desktop app</span>
</div>

<div class="assistant-note">
Guide the user through one numbered section at a time and wait for confirmation. Do not ask the user to open Terminal. If a label differs from this page, ask the user to describe what they see rather than guessing. Stop if the download is not from <strong>chatgpt.com</strong> or <strong>openai.com</strong>.
</div>

Codex is part of the ChatGPT desktop app. You do not need an API key or a separate model-provider account.

## 1. Check your macOS version

1. Select the Apple menu at the top-left of the screen.
2. Select **About This Mac**.
3. Look for the macOS version number.

Continue if it is macOS 14 or later. If it is older, use **System Settings > General > Software Update** before installing the app. If the Mac says it is up to date but still shows an older version, that Mac cannot use the Codex desktop route in this guide.

You do not need to identify whether the Mac has an Intel or Apple processor. The official download page handles that choice.

## 2. Make a folder for the first project

1. Open **Finder**.
2. Select **Documents** in the sidebar.
3. Choose **File > New Folder** from the menu bar.
4. Name the folder `Agent Projects`.
5. Open `Agent Projects` and create another new folder inside it.
6. Name the new folder `my-start-page`.

Codex will receive access to `my-start-page`, not the whole Documents folder or even the parent `Agent Projects` folder. For future projects, make and select a separate folder for each one.

## 3. Install the official app

<a class="button" href="https://chatgpt.com/download/">Open the official ChatGPT download page</a>

1. Download the app for macOS.
2. Open the downloaded disk image from the Downloads folder.
3. If a window asks you to move ChatGPT into **Applications**, do so.
4. Open **Applications** in Finder, then open **ChatGPT**.
5. If macOS asks whether to open an app downloaded from the internet, confirm only if the app came from the official page above.

If ChatGPT is already installed, open it and install any offered update instead.

## 4. Sign in

1. Select **Continue to sign in**.
2. Complete sign-in in the browser window that opens.
3. Use the same ChatGPT account as your subscription.
4. Return to the desktop app when the browser finishes.

Do not choose API-key authentication. API keys use separate billing and are not needed for this guide.

## 5. Open Codex in your safe folder

1. Open **Codex** in the ChatGPT desktop app.
2. Choose the option to create or open a local project.
3. Select **Documents > Agent Projects > my-start-page** as its folder.
4. Keep the permission setting on **Ask for approval**.

The precise button wording may change as the app is updated. The important result is a local Codex conversation whose selected folder is `my-start-page`.

**Ask for approval does not mean Codex asks before every file change.** It can normally create and edit files and run routine commands inside the selected folder. It asks before actions such as using the network or reaching outside that folder. Selecting one empty project folder keeps that automatic access narrow.

<div class="notice">
  <strong>Optional Mac permissions are not needed.</strong>
  This first project does not require Screen Recording, Accessibility, or control of other applications. Leave those features off if they are offered.
</div>

<div class="checkpoint">
  <strong>Checkpoint</strong>
  You should now see a new Codex conversation with <code>my-start-page</code> as its local folder. Do not paste the setup prompt into ordinary ChatGPT chat; paste it into this Codex conversation.
</div>

<div class="next-step">
  <h2>Move into the local agent</h2>
  <p>The browser assistant has finished its part. The next page contains the handoff prompt for Codex.</p>
  <a class="button" href="../handoff/">Continue to the handoff</a>
</div>
