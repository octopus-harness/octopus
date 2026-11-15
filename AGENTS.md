# octopus — agent guide

Personal reference repo. Every file is a hand-maintained list; append to them rather than rewriting:

| File | Contents |
| --- | --- |
| `README.md` | Repo overview and links |
| `cli.md` | Installed CLI / TUI clients |
| `mcps.md` | Installed MCP servers and their tools |
| `COMMANDS.md` | The `$$` command registry |

## `$$` commands

A message that begins with `$$` is a command, not a normal request. Handle it like this:

1. Parse `$$name [args…]` from the start of the message. Command names are case-insensitive; the rest of the message is arguments.
2. Open `COMMANDS.md` and find the `## $$name` section. That section is the source of truth for the response.
3. Reply with exactly what the section specifies — no preamble, no trailing commentary, no file edits, and no tool calls unless the section says otherwise.
4. If the command is not registered, reply with one line: `Unknown command: $$name. Run $$commands to see what's available.`
5. A bare `$$` is the same as `$$help`.

Only the first token counts: `$$commands please` runs `$$commands` and ignores `please` unless the command takes arguments.

## Adding a command

1. Add a row to the index table at the top of `COMMANDS.md`.
2. Add a `## $$name` section with its usage, arguments, and exact response format.

Keep the index table and the sections in the same order.
