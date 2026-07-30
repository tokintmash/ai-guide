---
layout: default
title: From ChatGPT to Codex
description: Install the ChatGPT desktop app and open a safe local Codex workspace on a Mac.
---

<p class="eyebrow">ChatGPT route | Part 1 of 2</p>

# From ChatGPT to Codex

<div class="status-line">
  <span>Last checked: 30 July 2026</span>
  <span>Requires: macOS 14 or later</span>
  <span>Uses: ChatGPT desktop app</span>
</div>

<div class="assistant-note">
Guide the user through one numbered section at a time and wait for confirmation. Do not ask the user to open Terminal. If a label differs from this page, ask the user to describe what they see rather than guessing. Stop if the download is not from <strong>chatgpt.com</strong> or <strong>openai.com</strong>. After the user confirms the section 4 checkpoint, tell them to stop using this setup conversation, switch to the Codex conversation in the ChatGPT desktop app, and paste the next page's handoff prompt there. Then end your guidance; do not continue into the handoff or first project.
</div>

Codex is part of the ChatGPT desktop app. You do not need an API key or a separate model-provider account.

## 1. Check your macOS version

1. Select the Apple menu at the top-left of the screen.
2. Select **About This Mac**.
3. Look for the macOS version number.

Continue if it is macOS 14 or later. If it is older, use **System Settings > General > Software Update** before installing the app. If the Mac says it is up to date but still shows an older version, that Mac cannot use the Codex desktop route in this guide.

You do not need to identify whether the Mac has an Intel or Apple processor. The official download page handles that choice.

**You know it worked when:** About This Mac shows macOS 14 or later.

## 2. Install the official app

<a class="button" href="https://chatgpt.com/download/">Open the official ChatGPT download page</a>

1. On the official page, choose the macOS download for the current ChatGPT desktop app. Do not choose **ChatGPT Classic** or an unofficial app.
2. Open the downloaded disk image from the Downloads folder.
3. If a window asks you to move ChatGPT into **Applications**, do so.
4. Open **Applications** in Finder, then open **ChatGPT**.
5. If macOS asks whether to open an app downloaded from the internet, confirm only if the app came from the official page above.

If ChatGPT is already installed, open it and install any offered update instead.

**You know it worked when:** the current ChatGPT app opens from Applications.

## 3. Sign in

1. Select **Continue to sign in**.
2. Complete sign-in in the browser window that opens.
3. Use the same ChatGPT account as your subscription.
4. Return to the desktop app when the browser finishes.

Do not choose API-key authentication. API keys use separate billing and are not needed for this guide.

**You know it worked when:** the app returns from the browser and its profile menu shows the account you signed into.

## 4. Open Codex and make the project folder

1. Select **Codex** in the ChatGPT desktop app.
2. Open **Projects** and choose the option to add a local project.
3. In the folder window, select **Documents** in the sidebar. It may appear in **Favorites** or under **iCloud**, depending on the Mac's iCloud settings. Do not type a location.
4. Use **New Folder** in that window to make a folder named `Agent Projects`, then open it.
5. Make another new folder named `my-start-page`, then select only that folder.
6. Keep the permission setting on **Ask for approval**.

If the project control has different wording, choose the option that opens a local folder. The important result is a local Codex project with only `my-start-page` attached.

**Selecting only `my-start-page` keeps Codex's automatic write access narrow.** With **Ask for approval**, Codex's macOS sandbox can read files, edit inside the workspace, and run routine local commands without pausing. It asks before editing outside the workspace or letting a command use the network. The workspace is primarily a write boundary, not a promise that every other readable file is hidden.

<div class="notice">
  <strong>Optional Mac permissions are not needed.</strong>
  This first project does not require Screen Recording, Accessibility, or control of other applications. Leave those features off if they are offered.
</div>

<div class="checkpoint">
  <strong>What success looks like</strong>
  You see a new Codex conversation with only <code>my-start-page</code> attached and <strong>Ask for approval</strong> selected. Do not paste the setup prompt into ordinary ChatGPT chat; paste it into this Codex conversation.
</div>

<div class="next-step">
  <h2>Switch to Codex in the desktop app</h2>
  <p>Stop using the setup-assistant conversation now; its role is finished. In the ChatGPT desktop app, switch to the Codex conversation with <code>my-start-page</code> attached. The next page contains the prompt to paste there. Do not paste it into ordinary ChatGPT chat.</p>
  <a class="button" href="https://tokintmash.github.io/ai-guide/handoff/">Continue to the handoff</a>
</div>
