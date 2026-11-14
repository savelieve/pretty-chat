# Pretty Chat

Give every conversation a little personality. Pretty Chat is an agent skill for clear, searchable conversation titles, with optional symbols, emoji, tags, and text styles.

## Get started

1. Copy `skills/pretty-chat` into your Codex skills directory: `~/.codex/skills/pretty-chat` (on Windows, `%USERPROFILE%\.codex\skills\pretty-chat`).
2. Start a new conversation and ask: **Use `$pretty-chat` to help me set up conversation naming.**
3. Describe your work or the kinds of chats you have, then choose a style. Review the suggested categories and symbols and change anything you like.
4. If you want the style available in future chats, choose a user-wide or workspace instruction file when the agent offers to save it. Otherwise, the choices apply to the current conversation.

For example, a designer might choose `✦` for design, `⌕` for research, and `✎` for content. A teacher might choose `◆` for lesson plans and `○` for student resources. These are examples, not required categories.

To encourage naming in every new chat, add an instruction to the relevant `AGENTS.md` asking the agent to use `$pretty-chat` for conversation titles. Skill selection and automatic execution depend on your host and configuration; neither this instruction nor installing the skill guarantees it will run in every chat.

## How it works

Pretty Chat uses your preferences to name the conversation around its goal. It respects a title you chose, and can update an automatic title when the topic changes if your preferences and host allow it. If a title tool is available, the agent can rename the chat and report the result. Otherwise, it gives you a title to copy.

Unicode symbols and text effects can look different across devices and may affect search, copying, or accessibility. Plain text is always an option. The skill cannot embed custom images or control icon colors in a plain-text title. Automatic token usage and cost counters are not included.

## Testing

Use the scenarios in [tests/scenarios.md](tests/scenarios.md) to evaluate behavior in a host with and without a title tool. The manifest validator checks the skill's structure but cannot establish that an agent follows its instructions or that a host renders characters correctly.

## Privacy

The skill contains instructions only. It does not include analytics, collect chat contents, or require an external service. Your agent and host may have their own data practices.
