# $$ Commands

Messages that begin with `$$` run the matching command from this file. Rows are listed in display order; `$$commands` prints them in this order.

## Index

| Command | Args | Description |
| --- | --- | --- |
| `$$commands` | — | List all available commands |
| `$$help` | `[command]` | Show the help message, or details for one command |
| `$$content_prompt` | — | Pull todos from `content-ideas` in doer-tui, pick one, and draft an article prompt |
| `$$readable_summary` | `[text]` | Rewrite the provided text into a concise, readable summary in the user's voice |

## $$commands

Usage: `$$commands`

Reply with the line `4 commands available:` followed by a Markdown table with the columns
`Command`, `Args` and `Description`, copied from the index above in the same order.
Nothing before or after it.

## $$help

Usage: `$$help [command]`

**Without an argument**, print this help message:

```text
`$$` commands — a message that begins with `$$` runs the matching command.

Usage: $$<command> [args]

Commands:
  $$commands            List all available commands
  $$help                Show the help message, or details for one command
  $$help <command>      Show details for one command
  $$content_prompt      Pull todos from `content-ideas` in doer-tui, pick one, and draft an article prompt
  $$readable_summary    Rewrite provided text into a readable summary in the user's voice

Example: $$help $$commands

Add or change commands in COMMANDS.md.
```

**With an argument**, strip a leading `$$` from the argument and match it case-insensitively
against the index:

- If it matches, print that command's section (usage, arguments, example) on its own,
  without the rest of the commands.
- If it doesn't match, reply with one line: `Unknown command: <arg>. Run $$commands to see what's available.`

## $$content_prompt

Usage: `$$content_prompt`

Tool use is allowed for this command.

1. Use `doer-tui` (or available `doer` tools) to locate the todo list named `content-ideas` and fetch its current todo items.
   - If `content-ideas` cannot be found or has no actionable items, reply with one line explaining that and stop.
2. Present the fetched items as a numbered list and ask the user which single item to work on. Use the `question` tool if available; otherwise ask directly in the reply and wait for their choice.
3. Once the user selects an item, produce a ready-to-use **article prompt** for that idea. The prompt should include, at minimum:
   - Working title
   - Target audience
   - Goal/thesis
   - Suggested outline (3–6 sections with brief bullet points)
   - Tone/style notes
   - Any key points or research angles implied by the selected todo
4. Do not modify files unless the user explicitly asks to save the generated prompt.

## $$readable_summary

Usage: `$$readable_summary [text]`

1. If the user provided text in the message, use that. Otherwise, ask the user to paste the text they want summarized and wait for their response.
2. Rewrite the text into a concise, readable summary. Match the user's voice: clear, direct, conversational — no corporate fluff or filler.
3. Return the summary. Do not modify files unless explicitly asked.
