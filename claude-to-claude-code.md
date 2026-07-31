---
layout: default
title: Set Up Claude Code in the Claude App
description: Install the Claude desktop app and open a safe local Claude Code session in its Code tab on a Mac.
---

<p class="eyebrow">Claude route | Part 1 of 2</p>

# Set up Claude Code in the Claude app

<div class="status-line">
  <span>Last checked: 30 July 2026</span>
  <span>Guide requires: macOS 13.5 or later</span>
  <span>Uses: Code tab in the Claude desktop app</span>
</div>

<div class="assistant-note">
Guide the user through one visible action at a time and wait for confirmation. Do not ask the user to open Terminal. If a label differs from this page, ask the user to describe what they see rather than guessing. Stop if the download is not from <strong>claude.com</strong> or <strong>claude.ai</strong>. After the user confirms the section 4 checkpoint, tell them to stop using this setup conversation, switch to the Claude Code session in the Code tab of the Claude desktop app, and paste the next page's handoff prompt there. Then end your guidance; do not continue into the handoff or first project.
</div>

The installed app is named **Claude**. Its **Code** tab runs Claude Code directly in the desktop app. Claude Code is also available as a separate command-line interface, but this guide does not install or use that CLI.

## 1. Check your macOS version

1. Select the Apple menu at the top-left of the screen.
2. Select **About This Mac**.
3. Look for the macOS version number.

This guide's first project uses the current Node.js LTS release, which requires macOS 13.5 or later. If the Mac is older, use **System Settings > General > Software Update** before continuing. If the Mac says it is up to date but still shows an older version, that Mac cannot use this edition of the guide.

You do not need to identify whether the Mac has an Intel or Apple processor. Claude's official Mac installer supports both.

**You know it worked when:** About This Mac shows macOS 13.5 or later.

## 2. Install the official app

<a class="button" href="https://claude.com/download">Open the official Claude download page</a>

1. Download Claude for macOS.
2. Open the downloaded disk image from the Downloads folder.
3. Move Claude into **Applications** if prompted.
4. Open **Applications** in Finder, then open **Claude**.
5. If macOS asks whether to open an app downloaded from the internet, confirm only if the app came from the official page above.

If Claude is already installed, open it and install any offered update instead.

**You know it worked when:** Claude opens from Applications.

## 3. Sign in

1. Sign in with the same Claude account as your subscription.
2. Complete any browser sign-in requested by the app.
3. Return to the Claude desktop app.
4. Open the **Code** tab.

If you see an upgrade message instead of Code, first check that the app is using the same account as your Claude subscription.

**You know it worked when:** the **Code** tab opens in the Claude desktop app.

## 4. Start a Claude Code session and make the project folder

1. In the **Code** tab, choose **Local**.
2. Select **Select folder**.
3. In the folder window, select **Documents** in the sidebar. It may appear in **Favorites** or under **iCloud**, depending on the Mac's iCloud settings. Do not type a location.
4. Use **New Folder** in that window to make a folder named `Agent Projects`, then open it.
5. Make another new folder named `my-start-page`, then select only that folder.
6. Keep the permission mode on **Manual**.

Claude uses `my-start-page` as its working directory, but it is not a hard filesystem sandbox. Anthropic says the **Code** tab has direct access to local files; **Manual** controls approvals and asks before edits and commands. Selecting one empty project folder keeps the intended scope clear. Reject requests to reach outside it unless you understand the reason.

<div class="notice">
  <strong>Optional Mac permissions are not needed.</strong>
  This first project does not require Screen Recording, Accessibility, or control of other applications. Leave computer-use features off if they are offered.
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
