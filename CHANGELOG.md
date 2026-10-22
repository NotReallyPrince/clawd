# Changelog

## 1.0.1

- **New logo:** the Bracket Crab, a pixel crab whose claws are code brackets. It's used for the Marketplace icon,
  the sidebar and tab icon, the status bar and the chat header.

## 1.0.0

Initial release of **Clawd — Agent Sidebar for Claude Code**: a Copilot-style coding agent in VS Code's secondary
sidebar, powered by your local Claude Code CLI and its login.

- **Several chats at once:** tabs, chats in editor tabs, a message queue, and chats that come back after a reload.
- **Context:** the current file and selection, `@` file mentions, files and folders, pasted images, and the `/` menu
  with every Claude Code command and your skills.
- **Controls:** Agent and Plan modes, model and effort pickers, an Ultracode switch for multi-agent work, approval
  policies (Review, Ask, Bypass), a context meter, and plan usage in the status bar.
- **Every step visible:** reads, searches, edits with +/− counts, commands with their output, thinking, todos,
  sub-agents nested under their step, and background tasks that keep running.
- **Review and undo:** Keep or Undo each change in the editor, restore any checkpoint (including changes made by
  commands in a git repo), redo, edit a sent message, retry.
- **History shared with Claude Code:** every chat for the folder, searchable, with rename, delete and pins. Chats show
  up in `claude --resume` and in the Claude Code extension, and the other way round.
- **Browser tools:** Claude can open, read, click, type and take screenshots in its own Chrome, with a live view.
- **Git:** commit messages written from your diff.
