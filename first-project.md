---
layout: default
title: Build Your First Project
description: Ask Codex or Claude Code to build a personal local start page with Node.js on Mac or Windows.
---

<p class="eyebrow">First project | About 15 minutes</p>

# Build a personal start page

This project is a small website available only on your computer. It requires no account, database, deployment service, or third-party code packages.

You will see the full agentic loop: describe a result, let the agent create and run it, inspect the result, and ask for a revision.

## 1. Ask the agent to build it

Paste this into the same local Codex or Claude Code conversation that completed the handoff. Do not return to the old setup conversation or start a second agent:

```text
Build my first project directly in the selected `my-start-page` folder. Do not create another project folder and do not work outside the selected folder.

Before writing files, ask me these three questions, one at a time:

1. What title should appear on the page?
2. Which 3–6 links should it include? Ask for each link’s name and web address. If I describe link categories instead, choose suitable links and tell me what you chose.
3. Should it feel calm, colorful, or minimal?

After I answer all three questions, build a polished personal start page using plain HTML, CSS, and JavaScript. Make it work well on both laptop and phone-sized screens.

Do not use frameworks, external fonts, analytics, third-party packages, or remotely hosted page assets.

Add a very small local server named `server.mjs` using only Node.js built-in features. It must:

- Serve files only from the selected `my-start-page` folder.
- Listen on `127.0.0.1` only, so other devices on my network cannot reach it.
- Use port 3000.
- Return appropriate content types and a proper 404 response.

Start the server in a persistent, non-blocking terminal or preview session using exactly:

node server.mjs

Keep the server running independently so the chat remains responsive. Do not run it as a blocking foreground command.

Then test http://127.0.0.1:3000, verify that the page and its local assets load successfully, check both laptop and phone-sized layouts, and show me the local preview.

If port 3000 is already occupied, identify the process first. Do not stop an unrelated process without asking me.

Explain any approval request in plain language before asking me to accept it.
```

## 2. Review the plan and approvals

The agent should first ask for your preferences. Claude in Manual mode should request permission before edits and commands. Codex may perform routine actions inside the selected folder without a separate approval. The expected actions are:

- Create files inside the selected `my-start-page` folder.
- Run Node to start a local web server.
- Open or preview a local address such as `http://localhost:3000`.

Those actions fit this project. Stop and ask for an explanation if it proposes installing packages, accessing another personal folder, using a network address other than `127.0.0.1` or `localhost`, or publishing anything online.

<div class="notice">
  <strong>Windows may show a firewall question.</strong>
  This project uses only <code>127.0.0.1</code>, so it does not need inbound access from private or public networks. If Windows asks whether to let Node.js communicate through the firewall, choose <strong>Cancel</strong>. The local browser preview should still work.
</div>

## 3. Inspect the result

Check four things in the preview:

1. The title matches what you requested.
2. Each link opens the expected destination.
3. The page is readable and feels like your chosen style.
4. Making the window narrow does not hide or overlap important content.

Do not worry about reading the source code yet. Start by judging the result as you would any other application or webpage.

## 4. Ask for one revision

Choose something you genuinely want changed. For example:

```text
Make the most important link stand out more, and add a small live clock. Keep the current style. Test the page again when you finish.
```

If the app asks for approval, review the change before accepting it. If Codex applies the edit inside the folder without asking, inspect the visible result and ask it to explain or revise anything you do not want. This revision step is important: an agentic workflow is a conversation about an evolving result, not a single perfect prompt.

## 5. Finish cleanly

When you are done, say:

```text
Stop the local server if it is still running. Then summarize what we made, tell me where the project files are, and explain how I can open and continue this project in a future session. Do not make any more changes.
```

The files remain in **Documents > Agent Projects > my-start-page** in Finder or File Explorer. You can reopen that folder in Codex or Claude Code whenever you want to continue.

<div class="checkpoint">
  <strong>You have completed the guide.</strong>
  You installed a local agent, gave it a limited workspace, prepared a runtime, created working software, reviewed its actions, and requested a revision. That is the core agentic workflow.
</div>

## Good next projects

- A local page that organizes recipes or travel notes.
- A small calculator for a recurring household task.
- A viewer for a non-sensitive spreadsheet copied into its own folder under `Agent Projects`.
- A simple game that runs in the browser.

Keep the next project local and non-sensitive while you become comfortable reviewing the agent's actions.
