# Agentic Desktop Starter Guide

A desktop-only guide for ordinary Mac and Windows users who want to use Codex in the ChatGPT desktop app or Claude Code in the **Code** tab of the Claude desktop app and complete a first local project without operating command-line applications.

## Instructions for an AI assistant

If a user gives you this repository and asks for help setting up an agentic environment:

1. Determine whether the target computer runs macOS or Windows. Ask one short question if it is unclear.
2. On a Mac, ChatGPT follows [the raw Mac Codex guide](https://raw.githubusercontent.com/tokintmash/ai-guide/main/chatgpt-to-codex.md) and Claude follows [the raw Mac Claude Code guide](https://raw.githubusercontent.com/tokintmash/ai-guide/main/claude-to-claude-code.md).
3. On Windows, ChatGPT follows [the raw Windows Codex guide](https://raw.githubusercontent.com/tokintmash/ai-guide/main/windows-chatgpt-to-codex.md) and Claude follows [the raw Windows Claude Code guide](https://raw.githubusercontent.com/tokintmash/ai-guide/main/windows-claude-to-claude-code.md).
4. Guide the user through one action at a time and wait for confirmation.
5. Assume the user can install desktop applications and navigate folders but does not operate Terminal, PowerShell, or Command Prompt.
6. Never ask the user to paste a password, API key, recovery code, or other secret.
7. Use only the official download pages linked by the guide.
8. Do not substitute a CLI, Homebrew, winget, WSL, version manager, shell script, API account, or third-party application.
9. Keep local work inside the single selected folder named `my-start-page`.
10. When the user confirms that the selected project folder and its coding chat or session are ready, explicitly tell them to stop using your setup conversation and switch to the Codex chat in the ChatGPT desktop app or the Claude Code session in the **Code** tab of the Claude desktop app. Send them to [the handoff guide](https://tokintmash.github.io/ai-guide/handoff/), then end your guidance. Do not perform, paraphrase, or continue into the handoff, Node.js check, or first project; that coding chat or session owns those steps.

If screen labels differ, ask the user to describe what they see. Do not invent a button or skip verification.

After the handoff, if the desktop coding agent reports that Node.js is missing, the user follows the graphical-install guide for [Mac](https://raw.githubusercontent.com/tokintmash/ai-guide/main/install-node-mac.md) or [Windows](https://raw.githubusercontent.com/tokintmash/ai-guide/main/install-node-windows.md) and then returns to that same Codex chat or Claude Code session. The [raw safety rules](https://raw.githubusercontent.com/tokintmash/ai-guide/main/safety.md) and [raw troubleshooting page](https://raw.githubusercontent.com/tokintmash/ai-guide/main/troubleshooting.md) are also directly fetchable.

## Human starting points

- [Set up a Mac](https://tokintmash.github.io/ai-guide/mac/)
- [Set up a Windows PC](https://tokintmash.github.io/ai-guide/windows/)
- [Read the five safety rules](https://tokintmash.github.io/ai-guide/safety/)

The public website is built directly from these Markdown files with GitHub Pages. The assistant links above use `raw.githubusercontent.com` because it serves plain Markdown directly, without relying on GitHub's file viewer or relative-link handling.

## Guide scope

- Desktop applications only
- Mac users on a supported macOS version
- Windows users on a supported Windows 11 PC
- A ChatGPT account with access to Codex in the desktop app, or a paid Claude plan with access to the desktop app's **Code** tab
- Graphical installers only
- Node.js, using the official LTS installer when it is missing
- One local, dependency-free example project

This edition assumes the required product access and does not compare plan availability. It intentionally excludes account setup, API keys, model-provider selection, user-operated command lines, package managers, WSL, Python, online deployment, computer control, and autonomous permission modes.

## Publishing with GitHub Pages

1. Create a public GitHub repository named `ai-guide` and leave the automatic README option off.
2. On the empty repository page, choose **uploading an existing file**.
3. Drag the contents of this folder into the upload area, including `_layouts` and `assets`.
4. Choose **Commit changes** after the upload finishes.
5. Open the repository's **Settings > Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the default branch and the root (`/`) folder.
8. Save and wait for GitHub to display the public site address.

The repository URL is enough for the setup assistant to choose a route. The handoff page gives the agent in the Codex chat or Claude Code session the constraints and context it needs for the later steps.

The included `_config.yml` assumes the repository is named `ai-guide`. If you publish a copy under another account, repository name, or domain, update `baseurl` and the canonical `tokintmash` URLs in the Markdown and `llms.txt`.

## Maintenance

The Windows ChatGPT and Codex instructions were last reviewed on **29 July 2026**. See [the raw source list](https://raw.githubusercontent.com/tokintmash/ai-guide/main/sources.md) for the official references and maintenance rules.
