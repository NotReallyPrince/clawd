# Changelog

## 1.0.3

- **Cleaner `/compact`:** a `/compact` message no longer shows the edit, retry or restore-checkpoint buttons, because
  there is nothing to edit, retry or undo. The "Conversation compacted" notice stays.
- **Fix:** a chat no longer disappears from history after Undo, Restore or a compaction makes a new copy that has
  no message of its own yet. The chat stays listed, and its pin stays put, until you send something in the copy.
- **Agent Changes view:** files waiting for Keep or Undo now show in their own "Agent Changes" section of the
  Source Control sidebar, with each file's folder and +/− counts, instead of as a "Clawd" repository among your git
  repos. Keep or Undo a file inline, or all of them from the section's title (Undo All asks first).
- **Browser tools switch:** turn Claude's browser tools on or off from the model menu, under Ultracode, instead of in
  Settings. A globe next to the model name shows they're on. It applies to every chat from its next message, and
  turning it back on returns to the window or headless mode you had.
- **Fewer compactions:** chats now compact on their own at 500k tokens instead of 200k. At 200k, the ~30–90k that
  every chat starts with left so little room that long chats compacted every few dozen replies. Change it under
  Settings → Clawd: Auto Compact At.

## 1.0.2

- **Crowned logo:** the Bracket Crab now wears a gold crown with a small gap above its head, and has shaded legs.
  The light bar across the top of the head is gone.
- **Sharper small logo:** the sidebar, tab and status bar icons use a simplified crab with bolder brackets and
  bigger eyes, so it no longer blurs into a blob at 16px.

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
