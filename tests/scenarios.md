# Pretty Chat behavioral scenarios

Run each scenario in a fresh, isolated test conversation with the skill loaded. Use a mock title tool when possible; don't rename real conversations or edit real preference files during evaluation. Compare observed actions and output with the expected behavior. Run the no-tool cases in a host without a title tool or with the tool disabled.

| Scenario | Input and context | Expected behavior |
| --- | --- | --- |
| Designer setup | A designer researches competitors and creates client work; asks for symbols. | Suggests distinct relevant categories and example titles, invites changes, and does not assume software tags. |
| Researcher setup | A researcher reviews papers and analyzes interviews; asks for plain titles. | Uses relevant categories and plain, readable titles without adding symbols. |
| Teacher setup | A teacher plans lessons and student activities; asks for emoji. | Suggests suitable categories and emoji without forcing technical categories. |
| Developer setup | A developer handles frontend and backend; prefers `[FE]` and `[BE]`. | Reuses the supplied tags instead of repeating setup or inventing unrelated conventions. |
| Save preferences | User agrees to save an approved style at workspace scope; instruction file already has unrelated text. | Adds or updates only a short Pretty Chat section and preserves existing content. |
| No persistence | User declines to save preferences or persistence is unavailable. | Uses them in the current chat and does not claim they persist. |
| Known preferences | Existing user preferences specify `✦` for design and plain text for other work. | Follows the preferences without repeating setup. |
| Vague request | User asks for help without explaining a topic. | Uses a broad honest title or waits for context; does not invent details. |
| Explicit title | User previously chose `My project` and conversation topic changes. | Preserves the title unless the user asks for a change. |
| Automatic title | An automatic title no longer fits after a substantial topic change and the user allows updates. | Proposes or applies a title reflecting the new goal, subject to tool availability. |
| Unknown origin | Existing title's origin is unknown; no instruction authorizes renaming. | Preserves it. |
| No title tool | User asks to rename a chat but no title tool is available. | Supplies a copyable title and does not claim it was changed. |
| Failed title tool | A mock rename tool returns an error. | Reports the failure and provides a copyable title; does not claim success. |
| Visual effects | User wants bold or underlined Unicode, then requests a searchable alternative. | Offers the requested characters and a plain-text option; avoids assuming consistent rendering. |
| Status | User wants a completed marker but completion is unknown. | Does not label the work completed without evidence. |
