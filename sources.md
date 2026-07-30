---
layout: default
title: Official Sources
description: Official product documentation used to maintain the Agentic Desktop Starter Guide.
---

<p class="eyebrow">Maintenance reference</p>

# Official sources

The Mac onboarding routes were last reviewed on **30 July 2026**; the Windows Codex route was last reviewed on **29 July 2026**. Interfaces and requirements change, so check these sources before revising the guide.

## OpenAI

- [Download ChatGPT](https://chatgpt.com/download/)
- [ChatGPT macOS app requirements](https://help.openai.com/en/articles/9275200-using-the-chatgpt-macos-app)
- [Codex app documentation](https://developers.openai.com/codex/app/)
- [Codex on Windows](https://developers.openai.com/codex/windows/windows-app)
- [Codex Windows sandbox](https://developers.openai.com/codex/windows/windows-sandbox)
- [ChatGPT Windows deployment and installers](https://developers.openai.com/codex/enterprise/windows-deployment)
- [Codex authentication](https://developers.openai.com/codex/auth/)
- [Codex projects and local folders](https://developers.openai.com/codex/projects/)
- [Codex permission modes](https://developers.openai.com/codex/permission-modes/)
- [Codex sandbox](https://developers.openai.com/codex/sandboxing/)

## Anthropic

- [Download Claude Desktop](https://claude.com/download)
- [Install Claude Desktop](https://support.claude.com/en/articles/10065433-install-claude-desktop)
- [Deploy Claude Desktop for Windows](https://support.claude.com/en/articles/12622703-deploy-claude-desktop-for-windows)
- [Claude Code desktop quickstart](https://code.claude.com/docs/en/desktop-quickstart)
- [Claude Code desktop reference](https://code.claude.com/docs/en/desktop)
- [Claude Code permissions](https://code.claude.com/docs/en/permissions)
- [Claude Code authentication](https://code.claude.com/docs/en/authentication)

## macOS folders

- [Desktop and Documents in iCloud Drive](https://support.apple.com/en-us/109344)
- [Create folders on Mac](https://support.apple.com/guide/mac-help/organize-files-with-folders-mh26885/mac)

## Node.js

- [Download Node.js](https://nodejs.org/en/download)
- [Node.js release schedule](https://github.com/nodejs/Release#release-schedule)
- [Supported Node.js platforms](https://github.com/nodejs/node/blob/main/BUILDING.md#platform-list)

## Windows prerequisites

- [Download Git for Windows](https://git-scm.com/download/win)
- [WinGet and App Installer](https://learn.microsoft.com/en-us/windows/package-manager/winget/)
- [Install and update App Installer](https://learn.microsoft.com/en-us/windows/msix/app-installer/install-update-app-installer)
- [App Installer in Microsoft Store](https://apps.microsoft.com/detail/9nblggh4nns1)
- [OneDrive Known Folder Move](https://learn.microsoft.com/en-us/sharepoint/redirect-known-folders)
- [Windows file and folder naming](https://learn.microsoft.com/en-us/windows/win32/fileio/naming-a-file)
- [Create a new folder in Windows](https://support.microsoft.com/en-us/windows/create-a-new-folder-cbbfb6f5-59dd-4e5d-95f6-a12577952e17)
- [Windows 10 support lifecycle](https://support.microsoft.com/en-us/windows/windows-10-support-ends-on-october-14-2025-2ca8b313-1946-43d3-b55c-2b95b107f281)
- [Windows Installer and User Account Control](https://learn.microsoft.com/en-us/windows/win32/msi/using-windows-installer-with-uac)

## Maintenance principles

- Link to stable download pages rather than versioned installer files.
- Say **LTS** instead of embedding a Node version in beginner instructions.
- Test the complete flow with new macOS and Windows 11 user accounts.
- Keep processor details out of the Mac path. Check x64 versus ARM64 on Windows because Claude, Git, and Node may provide separate installers.
- Update the "last checked" date only after testing or verifying all linked requirements.
