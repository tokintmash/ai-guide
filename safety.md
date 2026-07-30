---
layout: default
title: Five Safety Rules
description: Five practical safety rules for beginning to work with a desktop coding agent on Mac or Windows.
---

<p class="eyebrow">Read before setup | 3 minutes</p>

# Five safety rules

A coding agent can create files and run software on your behalf. Treat its requests much as you would requests from a helpful but newly hired assistant: give it a clear workspace, review unusual actions, and keep secrets private.

## 1. Start with one folder

When your route tells you to prepare a workspace, create `Agent Projects`, then `my-start-page`, inside Documents. Select only `my-start-page` as the workspace. If Windows places Documents under OneDrive, do not select OneDrive itself. Do not select the parent folder, your entire user folder, Documents, a photo library, email, or password-manager data.

If the agent needs another file, copy a non-sensitive version into the project folder rather than granting broad access.

The coding agent may send prompts and relevant content from the selected project to its AI service for processing. Selecting one local folder clearly defines the intended working scope, but it is not a hard sandbox in every app. Reject requests to reach outside it. A local project also does not make the AI service offline.

## 2. Install from official sources

This guide links to `chatgpt.com`, `claude.com`, `nodejs.org`, and, on the Windows Claude route, `git-scm.com`. Check the address before downloading.

For this beginner setup, reject instructions that ask you to paste an installation command, run `curl`, install Homebrew, use winget or Chocolatey, or disable an operating-system security feature. Those tools can be legitimate, but they are not part of this guide.

## 3. Keep secrets out of chat

Never paste these into an AI conversation:

- Your computer password or account password.
- A two-factor authentication or recovery code.
- An API key or private cryptographic key.
- Banking, medical, identity, or confidential workplace data.

It is normal to approve a genuine macOS Installer or Windows User Account Control dialog. If administrator credentials are required, enter them only in the operating system's own security dialog. The agent should not ask to see them.

## 4. Review unusual actions

Version checks, creating files in the selected project folder, and starting the local project are expected. Pause when an action would:

- Access a folder outside `my-start-page`.
- Delete many files or replace existing work.
- Upload, publish, email, purchase, or sign into something.
- Install software or change system settings.
- Request Accessibility, Screen Recording, or control of other apps.

Ask the agent what the action does, why it is needed, and what the safer alternative is. Reject it if the answer is unclear.

## 5. Keep a human decision point

For the first projects, use **Ask for approval** in Codex or **Manual** in Claude Code. These modes are not identical: Claude Manual asks before edits and commands, while Codex can perform routine work inside the selected folder without asking each time. Review the visible result and the app's record of file changes. Do not enable a less restrictive mode.

Use only one local-agent conversation for a project at a time. Before starting another conversation for `my-start-page`, tell the current agent to stop or wait and confirm that it has no task or local server still running.

An agent may make a confident mistake. You remain responsible for decisions that affect accounts, money, private information, other people, or important files.

<div class="notice">
  <strong>This guide intentionally does less.</strong>
  It does not enable computer control, broad file access, online publishing, API keys, or autonomous approval modes. Those can be explored later, one capability at a time.
</div>
