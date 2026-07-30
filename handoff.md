---
layout: default
title: Hand Off to the Local Agent
description: End the setup conversation, move to Codex or Claude Code, and check Node.js safely.
---

<p class="eyebrow">All routes | Part 2</p>

# Hand off to the local agent

This is the handoff boundary. Stop using the setup-assistant conversation; its role has ended. Keep this guide webpage open, switch to the desktop app, and paste the prompt below into the **Codex local project** or **Claude Code session** with `my-start-page` selected.

<div class="notice">
  <strong>The conversations are separate.</strong>
  The desktop coding agent cannot see the earlier setup conversation, even when both use the same account or app. From this point forward, use only this one local-agent conversation for the guide and project. Do not ask both AIs to continue.
</div>

<div class="assistant-note">
This page is for the separate local desktop coding agent, not the initial setup assistant. Continue only if you are inside a Codex local project or Claude Code session with <code>my-start-page</code> selected. Follow every constraint in the user's pasted prompt. Run checks yourself through your tools; never direct the user to a command-line application. Treat the selected folder as the workspace boundary.
</div>

## 1. Paste the setup prompt

```text
This is a new, separate local-agent conversation. My setup assistant has ended its role, and you cannot see its conversation history. The official desktop app is installed and signed in, the selected workspace is "my-start-page", the route's recommended permission mode is still selected, and no project work has started. You are the only AI I am asking to work on this local project.

I am following the Agentic Desktop Starter Guide (https://tokintmash.github.io/ai-guide/) and I do not operate command-line applications.

Work only inside the selected "my-start-page" folder unless you explain why another location is needed and I explicitly approve it. Explain meaningful actions in plain language. Ask before installing software, downloading code, deleting files, or changing system settings. Never ask me to paste a password, API key, recovery code, or other secret into chat.

First, check whether Node.js and npm are available. On macOS, run `node --version` and `npm --version`. On Windows, run `node --version` and `npm.cmd --version`. Run the appropriate checks yourself. These are read-only checks. Tell me the result in plain language.

If both are available, do not upgrade them and tell me I am ready for the first project.

If either is missing, do not install it through a shell, Homebrew, winget, Chocolatey, a version manager, curl, or a downloaded script. Tell me to use the official graphical installer for my current operating system at https://nodejs.org/en/download and wait while I do that. On Windows, make sure the MSI architecture matches the PC. After I return, check again. If the new installation is not visible, ask me to quit and reopen this desktop app, then check once more.
```

## 2. Review the first request

The agent should propose two read-only checks:

- `node --version` asks Node.js to report its version.
- `npm --version` on Mac or `npm.cmd --version` on Windows asks Node's package manager to report its version.

These checks do not change files. Approve them if the app asks.

## 3. Follow the result

If the agent reports version numbers for both tools, continue directly to the first project.

If the agent says either tool is missing, use the graphical Node installer page for your operating system. You will not need a command-line application.

<a class="button" href="https://tokintmash.github.io/ai-guide/first-project/">Node is ready: start the project</a>
<a class="button secondary" href="https://tokintmash.github.io/ai-guide/install-node/">Node is missing: install it</a>

<div class="checkpoint">
  <strong>What success looks like</strong>
  The agent reports a Node version beginning with <code>v</code> and a separate npm version number. The exact numbers will change over time and do not need to match a screenshot.
</div>
