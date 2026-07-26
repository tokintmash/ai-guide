---
layout: default
title: Hand Off to the Local Agent
description: Transfer setup from browser chat to Codex or Claude Code and check Node.js safely.
---

<p class="eyebrow">Both routes | Part 2</p>

# Hand off to the local agent

The conversation now moves from the browser assistant to the desktop coding agent. Keep this page open, but paste the prompt below into the **Codex local project** or **Claude Code session** you just created.

<div class="assistant-note">
You are now assisting inside a local desktop coding workspace. Follow every constraint in the user's pasted prompt. Run checks yourself through your tools; never direct the user to Terminal. Treat the selected <code>my-start-page</code> folder as the workspace boundary.
</div>

## 1. Paste the setup prompt

```text
You are my local desktop coding agent. I am following the Agentic Mac Starter Guide and I do not operate Terminal.

Work only inside the selected "my-start-page" folder unless you explain why another location is needed and I explicitly approve it. Explain meaningful actions in plain language. Ask before installing software, downloading code, deleting files, or changing system settings. Never ask me to paste a password, API key, recovery code, or other secret into chat.

First, check whether Node.js and npm are available by running `node --version` and `npm --version` yourself. These are read-only checks. Tell me the result in plain language.

If both are available, do not upgrade them and tell me I am ready for the first project.

If either is missing, do not install it through Terminal, Homebrew, a version manager, curl, or a downloaded script. Tell me to use the official graphical macOS installer at https://nodejs.org/en/download and wait while I do that. After I return, check again. If the new installation is not visible, ask me to quit and reopen this desktop app, then check once more.
```

## 2. Review the first request

The agent should propose two read-only checks:

- `node --version` asks Node.js to report its version.
- `npm --version` asks Node's package manager to report its version.

These checks do not change files. Approve them if the app asks.

## 3. Follow the result

If the agent reports version numbers for both tools, continue directly to the first project.

If the agent says either tool is missing, use the graphical Node installer page. You will not need Terminal.

<a class="button" href="../first-project/">Node is ready: start the project</a>
<a class="button secondary" href="../install-node/">Node is missing: install it</a>

<div class="checkpoint">
  <strong>What success looks like</strong>
  The agent reports a Node version beginning with <code>v</code> and a separate npm version number. The exact numbers will change over time and do not need to match a screenshot.
</div>
