# Agentic Desktop Starter Guide

A desktop-only guide for ordinary Mac and Windows users who want to move from ChatGPT to Codex, or from Claude to Claude Code, and complete a first local project without operating command-line applications.

## Instructions for an AI assistant

If a user gives you this repository and asks for help setting up an agentic environment:

1. Determine whether the target computer runs macOS or Windows. Ask one short question if it is unclear.
2. On a Mac, ChatGPT follows [`chatgpt-to-codex.md`](chatgpt-to-codex.md) and Claude follows [`claude-to-claude-code.md`](claude-to-claude-code.md).
3. On Windows, ChatGPT follows [`windows-chatgpt-to-codex.md`](windows-chatgpt-to-codex.md) and Claude follows [`windows-claude-to-claude-code.md`](windows-claude-to-claude-code.md).
4. Guide the user through one action at a time and wait for confirmation.
5. Assume the user can install desktop applications and navigate folders but does not operate Terminal, PowerShell, or Command Prompt.
6. Never ask the user to paste a password, API key, recovery code, or other secret.
7. Use only the official download pages linked by the guide.
8. Do not substitute a CLI, Homebrew, winget, WSL, version manager, shell script, API account, or third-party application.
9. Keep local work inside the single selected `Documents/Agent Projects/my-start-page` folder.
10. After the desktop agent is ready, continue with [`handoff.md`](handoff.md), then [`first-project.md`](first-project.md).

If screen labels differ, ask the user to describe what they see. Do not invent a button or skip verification.

## Human starting points

- [Set up a Mac](mac.md)
- [Set up a Windows PC](windows.md)
- [Read the five safety rules](safety.md)

The public website is built directly from these Markdown files with GitHub Pages. No local build step is required.

## Guide scope

- Desktop applications only
- Mac users on a supported macOS version
- Windows users on a fully updated, 64-bit Windows 11 PC
- Existing subscription assumed
- Graphical installers only
- Node.js, using the official LTS installer when it is missing
- One local, dependency-free example project

This edition assumes an existing subscription and does not compare plan availability. It intentionally excludes free-account setup, API keys, model-provider selection, user-operated command lines, package managers, WSL, Python, online deployment, computer control, and autonomous permission modes.

## Publishing with GitHub Pages

1. Create a public GitHub repository named `ai-guide` and leave the automatic README option off.
2. On the empty repository page, choose **uploading an existing file**.
3. Drag the contents of this folder into the upload area, including `_layouts` and `assets`.
4. Choose **Commit changes** after the upload finishes.
5. Open the repository's **Settings > Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the default branch and the root (`/`) folder.
8. Save and wait for GitHub to display the public site address.

The repository URL itself is enough for an AI assistant because this README contains routing instructions.

The included `_config.yml` assumes the repository is named `ai-guide`. If you use another repository name, change `baseurl` to `/<repository-name>`. For a root site or custom domain, set it to an empty string.

## Maintenance

Product instructions were last reviewed on **27 July 2026**. See [`sources.md`](sources.md) for the official references and maintenance rules.
