# Pretty Chat

Give every conversation a little personality. Pretty Chat is an agent skill that helps people choose clear, searchable conversation titles, with optional symbols, emoji, and text styles.

## Get started

1. Copy `skills/pretty-chat` into your Codex skills directory: `~/.codex/skills/pretty-chat` (on Windows, `%USERPROFILE%\.codex\skills\pretty-chat`).
2. Start a new conversation and ask: **Use `$pretty-chat` to help me set up conversation naming.**
3. Describe what you do and the kinds of chats you have. Pretty Chat will suggest categories and symbols that you can adjust.

To encourage naming in every new chat, add an instruction to your user or workspace `AGENTS.md` to use `$pretty-chat` for conversation titles. Skill selection and automatic execution depend on your host and configuration.

## How it works

The skill chooses concise titles based on your preferences. It can use Unicode symbols, emoji, text tags, or optional Unicode text effects. If the host provides a chat-title tool, the agent can use it; otherwise it can suggest a title for you to set. Rendering, search, and accessibility of styled characters vary by device and app.

The skill does not embed custom images or control icon colors. Automatic token usage and cost counters are not included; those remain an experimental local investigation and are not a supported feature.

## Privacy

The skill contains instructions only. It does not include analytics, collect chat contents, or require an external service. Your agent and host may have their own data practices.
