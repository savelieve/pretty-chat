---
name: pretty-chat
description: Set up personalized conversation naming or name and rename chats using a person's chosen style and the host's available tools.
---

# Pretty Chat

Give conversations concise, specific, searchable names in the user's preferred style. Follow explicit user and workspace instructions first. Avoid sensitive details; name the goal or subject, not merely "discussion". Do not invent a specific topic when the conversation is still vague.

## Set up a personal style

When asked to set up Pretty Chat, use known preferences and ask only for missing essentials: what the person does or uses chats for, and whether they prefer symbols, emoji, text tags, plain text, or a combination. Infer a small set of distinct categories suited to their activities and propose a character or tag for each, with example titles. Let them revise the suggestions. Do not force software categories on other kinds of work.

Use agreed preferences for the current chat. Offer to save them for future chats in a user-wide or workspace instruction file supported by the host; write only after the user chooses the scope. Preserve existing instructions and edit only the Pretty Chat section. If persistence is unavailable or declined, say that the style applies only in the current chat. Existing instructions and explicit user choices take precedence over this skill's suggestions.

Use a short, editable section such as:

```markdown
## Pretty Chat preferences
- Style: Unicode symbol and plain-language title
- Categories: ✦ design; ⌕ research; ✎ writing
- Renaming: update automatic titles when the main goal changes; keep titles I chose
```

Treat the example as a format, not as a default taxonomy. Do not store sensitive details just to name chats. When saved preferences are available, follow them without repeating setup; otherwise use existing workspace conventions or a plain descriptive title.

## Name the conversation

Choose a brief title that identifies the real task, such as `✦ Mobile checkout redesign`. Use one category marker where helpful; a second is optional when it clarifies the subject. Prefer stable topic meanings to unverified status labels. When the topic is unclear, use a broad honest title or wait for enough context.

Respect a title explicitly chosen by the user unless they ask to change it. If a title was automatically generated and the main purpose materially changes, update it when the user's preferences and host permit. If its origin is unknown, preserve it unless the user requests a rename or an applicable instruction authorizes it.

Use an available authorized conversation-title tool for the intended chat. Check its result before claiming success. If no such tool is available or the call fails, say so when relevant and provide a ready-to-copy title. A skill or persistent instruction can encourage automatic use but cannot guarantee invocation or title-tool access on every host.

## Visual styles

Use plain text, Unicode symbols, emoji, tags, or a combination according to the user's preferences. Suggest distinct, legible characters such as `◈`, `✦`, `⚙`, `⌘`, `✎`, `◆`, or `○` when they fit; let the user test and replace them. Do not rely on color to communicate meaning.

When requested, Unicode can approximate bold (`𝗕𝗼𝗹𝗱`), underline (`U̲n̲d̲e̲r̲`), and strikethrough (`S̶t̶r̶i̶k̶e̶`); these are characters, not rich formatting. Rendering varies, and styled characters can hinder searching, copying, or assistive technology. Offer ordinary text as an alternative. Do not imply completion or another status with strikethrough unless requested and known. Plain-text titles do not provide custom image assets or arbitrary icon colors.
