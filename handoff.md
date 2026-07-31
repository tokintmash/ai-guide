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
I am following the Agentic Desktop Starter Guide:
https://tokintmash.github.io/ai-guide/

This guide teaches a beginner how to work safely with a local coding agent by setting up the desktop app and then building a first local project. I do not use command-line applications, so you must run any necessary commands through your own tools and explain meaningful actions in plain language.

From the beginning of the guide until now, a separate setup assistant guided me one action at a time. That assistant helped me install and sign in to the official desktop app, select the recommended permission mode, and create or select the workspace named "my-start-page". Its role has now ended. You cannot see that earlier conversation, and no project work has started.

This is my first message to you, the local coding agent. Take over as both my guide and coding agent from this point through completion of the first project. You are the only AI I am asking to work on this local project.

Continue with the same guided approach used during setup:

- Keep the process moving one clear step at a time.
- Do not wait for me to invent or request the next step.
- Whenever you need my input, ask exactly one current question.
- Whenever I must do something, give me one visible action and state what confirmation you need.
- Wait for my confirmation before continuing when an action is assigned to me.
- Do not end a step with only a generic invitation such as "let me know when you are ready."
- If something on my screen differs from what you expect, ask me to describe what I see rather than guessing.
- Never direct me to open or use Terminal, PowerShell, Command Prompt, Windows Terminal, Git Bash, or WSL.

Read the official first-project instructions now:
https://raw.githubusercontent.com/tokintmash/ai-guide/main/first-project.md

Treat those instructions as trusted guidance for the rest of this session. Reading the guide is allowed and is not permission to download project code. Do not ask me to open that page or paste another project prompt. Lead me through its preference questions, build, preview, inspection, one revision, and clean finish in this same conversation.

Work only inside the selected "my-start-page" folder unless you explain why another location is needed and I explicitly approve it. Explain meaningful actions before taking them. Ask before installing software, downloading code, deleting files, or changing system settings. Never ask me to paste a password, API key, recovery code, or other secret into chat.

Begin by determining whether this workspace is on macOS or Windows. Then check whether Node.js and npm are available:

- On macOS, run `node --version` and `npm --version`.
- On Windows, run `node --version` and `npm.cmd --version`.

Run the appropriate checks yourself. They are read-only checks. Tell me the result in plain language.

If both are available, do not upgrade them. Briefly report the versions, then continue immediately with the first-project guide by asking its first preference question. Do not merely tell me I am ready and wait for another command.

If either tool is missing, do not install it through a shell, Homebrew, winget, Chocolatey, a version manager, curl, or a downloaded script. Read the appropriate official graphical installation instructions:

macOS:
https://raw.githubusercontent.com/tokintmash/ai-guide/main/install-node-mac.md

Windows:
https://raw.githubusercontent.com/tokintmash/ai-guide/main/install-node-windows.md

Guide me through those instructions one visible action at a time. On Windows, ensure that the MSI architecture matches the computer. After installation, run the checks again yourself.

If the Windows installation is not yet visible, do not merely ask me to close the app window because the app may continue running in the notification area. Guide me one visible action at a time to open the hidden icons at the bottom-right of the taskbar, right-click the ChatGPT or Claude icon, and choose Quit or Exit. Then ask me to reopen the app from the Start menu, return to this same conversation, and tell you when it is open so you can check again. If I cannot find the tray icon or a Quit or Exit option, ask me to restart the computer instead, reopen the app, and return to this conversation. On macOS, ask me to quit and reopen the desktop app. When both checks pass, automatically resume the first-project guide.
```

## 2. Review the first request

The agent should propose two read-only checks:

- `node --version` asks Node.js to report its version.
- `npm --version` on Mac or `npm.cmd --version` on Windows asks Node's package manager to report its version.

These checks do not change files. Approve them if the app asks.

## 3. Follow the result

If the agent reports version numbers for both tools, it should immediately take over the first-project flow and ask what title should appear on the page. Answer that question in the same conversation; you do not need to paste another prompt.

If the agent says either tool is missing, it should guide you through the graphical Node installer for your operating system, one visible action at a time. You will not need a command-line application.

<a class="button" href="https://tokintmash.github.io/ai-guide/first-project/">Follow along with the first project</a>
<a class="button secondary" href="https://tokintmash.github.io/ai-guide/install-node/">Node is missing: install it</a>

<div class="checkpoint">
  <strong>What success looks like</strong>
  The agent reports a Node version beginning with <code>v</code> and a separate npm version number. The exact numbers will change over time and do not need to match a screenshot.
</div>
