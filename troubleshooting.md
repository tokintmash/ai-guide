---
layout: default
title: Get Unstuck
description: Plain-language fixes for common Codex, Claude Code, Node.js, Mac, and Windows setup problems.
---

<p class="eyebrow">Troubleshooting | No command line required</p>

# Get unstuck

Describe what you see to the assistant that is guiding you. Include the exact wording of an error, but remove email addresses, account details, file contents, and other private information first.

## I cannot find Codex in ChatGPT

1. Confirm you installed the current app from [the official ChatGPT download page](https://chatgpt.com/download/).
2. Check for an app update.
3. Confirm the app is signed into the same account and workspace as your subscription.
4. Quit and reopen the app.

The current app combines ChatGPT and Codex. Do not install an unofficial app with "Codex" in its name.

## I cannot find Code in Claude Desktop

1. Confirm you installed the current app from [the official Claude download page](https://claude.com/download).
2. Check that the app is signed into the account with Claude Code access.
3. Install any offered app update.
4. Quit and reopen Claude.

Claude Chat and Claude Code are different workspaces in the same desktop app. This guide uses **Code**.

## Claude Code on Windows says Git is missing

1. Download Git only from the [official Git for Windows page](https://git-scm.com/download/win).
2. Run its graphical installer and keep the recommended options.
3. Quit Claude Desktop completely after installation.
4. Reopen Claude from the Start menu and return to Code.

You do not need to open Git Bash or type a Git command. Claude Code uses Git behind the scenes.

## macOS will not open the downloaded app

Delete the download and return to the official download page linked by this guide. Do not disable Gatekeeper or other Mac security features. If a work or school Mac blocks installation, its administrator may need to approve the app.

## My Mac is up to date but the version is too old

Some older Macs cannot install the macOS version required by the current desktop agent or Node.js. If Software Update says the Mac is up to date but **About This Mac** still shows a version below the guide's requirement, stop here. This desktop-only edition has no safe fallback for that Mac.

## Windows blocks the downloaded installer

Delete the installer and download it again from the official page linked by this guide. Do not turn off Microsoft Defender, bypass SmartScreen for an unknown publisher, or change a Windows security policy. A managed work or school PC may require its administrator to approve the app.

## I have Windows 10

This edition uses Windows 11 as its supported baseline. OpenAI describes Codex support on Windows 10 as best effort and requires version 1809 or newer in practice because Codex depends on modern console support. Open **Start**, select **Settings**, then select **Windows Update** and install the available Windows 10 updates before trying Codex. If the PC cannot run Windows 11, this guide does not provide a CLI or WSL fallback.

## Codex says WinGet is missing

WinGet is part of Microsoft's **App Installer** system component. Do not use the Installed apps list as the check and do not open a command-line application. Open [App Installer in the Microsoft Store](https://apps.microsoft.com/detail/9nblggh4nns1), then install or update it. Return to ChatGPT when the Store shows it as installed, then retry the Codex action that reported the error.

OpenAI says WinGet should be available, but this guide checks it only when Codex reports a problem rather than making it a routine gate. Codex's stronger Windows sandbox uses lower-privilege users, filesystem permissions, firewall rules, and local Windows policy; App Installer does not provide those sandbox protections.

## The app asks for file access

Allow access only when the dialog identifies the `my-start-page` folder you selected. If it asks for the parent `Agent Projects` folder, the whole Documents folder, your Windows user profile, or another personal location, cancel and return to the app's folder selection.

## The app asks to see or control other applications

Choose **Not Now**, **Deny**, or cancel. On Mac these may appear as Screen Recording or Accessibility permissions. Both desktop apps also have optional computer-control features. None are required for this guide.

## Node is still missing after installation

1. Confirm the macOS package installer or Windows MSI installer reported success.
2. Quit the entire ChatGPT or Claude desktop app.
3. On Mac, open the app again from Applications. On Windows, open it from the Start menu.
4. Reopen the local workspace.
5. Ask the agent to repeat the Node and npm version checks for the current operating system.

Do not install a second copy through another method. If the checks still fail, tell the agent whether you used the official `.pkg` or `.msi` and ask it to diagnose without changing anything.

## The agent wants me to use a command line

Reply with:

```text
I am following a desktop-only guide and will not operate Terminal, PowerShell, Command Prompt, Git Bash, or WSL. Run necessary read-only checks through your own tools. If an installation needs a graphical installer, give me the official page and guide me through the installer windows instead.
```

## The local preview does not open

Ask the agent to check whether its server is still running and whether it reported a different local address. A local address usually begins with `http://localhost:` followed by a number.

If the chosen number is already in use, the agent can stop its own process or choose another number. It should not stop unrelated applications without asking.

On Windows, the first Node.js server may trigger a Windows Firewall dialog. This guide's server listens only on `127.0.0.1` and does not need private or public network access, so choose **Cancel**. If the preview still fails, ask the agent to confirm that it used `127.0.0.1` and started the server directly with `node server.mjs`.

## The project looks broken

Tell the agent what is visibly wrong and ask it to inspect the browser errors, fix only the project files, and test again. You can reject a proposed change and ask for a smaller one.

## I approved something by mistake

Ask the agent to stop and explain exactly what changed. Do not ask it to "undo everything" until it has identified the affected files and actions. If private information may have been uploaded or a credential exposed, change that credential from the relevant service immediately.

For product-specific help, use the [official sources](https://tokintmash.github.io/ai-guide/sources/) rather than third-party download or support sites.
