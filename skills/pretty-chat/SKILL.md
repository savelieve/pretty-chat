---
name: pretty-chat
description: Name or rename a conversation with concise, searchable topic tags when requested or when a workspace rule calls for chat naming.
---

# Name conversations

Choose a concise, specific title that makes the conversation easy to find. Use the user's or workspace's naming conventions when supplied; otherwise use `[TAG] - Specific topic`, adding a second tag only when it helps. Avoid sensitive details and generic titles. Update the title if the conversation's main purpose materially changes, while respecting any title explicitly chosen by the user.

Suggested tags: `WP` workspace and process; `FE` frontend; `BE` backend; `DB` database; `GH` GitHub; `DC` deployment and infrastructure; `UX` design; `QA` testing; `BUG` investigation; `REL` releases; `DOC` documentation. Adapt the tags to the user's work rather than forcing a software category.

If an authorized chat-title tool is available, use it for the current conversation. Do not assume the host supports renaming or claim success without a successful tool result. If no such tool is available, suggest the title when the user asks. This skill alone cannot guarantee execution in every new chat: automatic use depends on the host's skill discovery or a persistent instruction to apply it.

## Personal setup

When a user wants to set up a naming style, ask briefly what they do and the kinds of conversations they want to organize. Use any preferences and context already provided; don't repeat setup in every chat. Ask whether they prefer symbols, emoji, text tags, plain titles, or a combination if that is not already clear.

For a symbol style, infer a small, distinct set of work categories and suggest one readable Unicode character for each, with a few example titles. Choose characters that fit the user's activities, such as `◈`, `✦`, `⚙`, `⌘`, `✎`, `◆`, or `○`; don't force a software-oriented taxonomy. Let the user change categories and symbols. Prefer stable topic meanings over inferred status, and don't rely on color to communicate meaning. Characters can render differently across devices, so offer to test and replace any that display poorly.

Use the agreed preferences in the current conversation. For reuse across chats, offer to save them in a suitable persistent user or workspace instruction file, respecting the user's chosen scope; don't claim preferences persist unless they were saved. When no preferences are available, use the existing workspace convention or a simple descriptive title.
## Optional visual styles

Offer plain text, emoji, tags, or a combination according to the user's preference. When requested, Unicode can approximate **bold** (mathematical bold characters, e.g. `𝗕𝗼𝗹𝗱`), underline (combining low line, e.g. `U̲n̲d̲e̲r̲`), and strikethrough (combining long stroke, e.g. `S̶t̶r̶i̶k̶e̶`). These are text characters, not rich-text formatting; Markdown and HTML need host support to render as formatting. Rendering varies across hosts and devices.

Use effects only when the user wants them, and keep titles concise and readable. Unicode styling can impair search, copying, and assistive technology; preserve an ordinary-text option. Do not use strikethrough to imply completion or another status unless the user requests that meaning and the status is known. A plain-text title tool does not itself provide custom icon assets or color controls; colored emoji are an optional visual cue.

