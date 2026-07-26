---
layout: default
title: Get Unstuck
description: Plain-language fixes for common Codex, Claude Code, Node.js, and local project setup problems.
---

<p class="eyebrow">Troubleshooting | No Terminal required</p>

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

## macOS will not open the downloaded app

Delete the download and return to the official download page linked by this guide. Do not disable Gatekeeper or other Mac security features. If a work or school Mac blocks installation, its administrator may need to approve the app.

## My Mac is up to date but the version is too old

Some older Macs cannot install the macOS version required by the current desktop agent or Node.js. If Software Update says the Mac is up to date but **About This Mac** still shows a version below the guide's requirement, stop here. This desktop-only edition has no safe fallback for that Mac.

## The app asks for file access

Allow access only when the dialog identifies the `my-start-page` folder you selected. If it asks for the parent `Agent Projects` folder, the whole Documents folder, or another personal location, cancel and return to the app's folder selection.

## The app asks for Screen Recording or Accessibility

Choose **Not Now**, **Deny**, or cancel. Those permissions support optional computer-control features and are not required for this guide.

## Node is still missing after installation

1. Confirm the macOS Installer reported success.
2. Quit the entire ChatGPT or Claude desktop app.
3. Open the app again from Applications.
4. Reopen the local workspace.
5. Ask the agent to run `node --version` and `npm --version` again.

Do not install a second copy through another method. If the checks still fail, tell the agent where the `.pkg` came from and ask it to diagnose without changing anything.

## The agent wants me to use Terminal

Reply with:

```text
I am following a desktop-only guide and will not operate Terminal. Run necessary read-only checks through your own tools. If an installation needs a graphical Mac installer, give me the official page and guide me through the windows instead.
```

## The local preview does not open

Ask the agent to check whether its server is still running and whether it reported a different local address. A local address usually begins with `http://localhost:` followed by a number.

If the chosen number is already in use, the agent can stop its own process or choose another number. It should not stop unrelated applications without asking.

## The project looks broken

Tell the agent what is visibly wrong and ask it to inspect the browser errors, fix only the project files, and test again. You can reject a proposed change and ask for a smaller one.

## I approved something by mistake

Ask the agent to stop and explain exactly what changed. Do not ask it to "undo everything" until it has identified the affected files and actions. If private information may have been uploaded or a credential exposed, change that credential from the relevant service immediately.

For product-specific help, use the [official sources](../sources/) rather than third-party download or support sites.
