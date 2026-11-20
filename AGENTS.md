# octopus: agent guide

Octopus is a personal command and workspace harness for AI agents. It uses lightweight CLI tools (`com` and `work`) to load specific Markdown context on demand (`$$` commands) and manage isolated workspaces.

| Path | Contents |
| --- | --- |
| `README.md` | Repo overview, ecosystem links, and quickstart |
| `COMMANDS.md` | How to use `com` for `$$` commands |
| `AGENTS.md` | Agent guide and `$$` command protocol |
| `commands/` | Local command Markdown files (gitignored) |
| `workspace/` | Active workspace folders (gitignored) |
| `archive/` | Archived workspace folders (gitignored) |

## `$$` commands

A message that begins with `$$` is a command, not a normal request. Handle it like this:

1. Parse `$$name [args...]` from the start of the message. Command names are case-insensitive; the rest of the message is arguments.
2. Run `com get <name>` (stripping the leading `$$`) to read `./commands/<name>.md`. That file is the source of truth for the response.
3. Reply with what the command file specifies: no preamble, no trailing commentary, no file edits, and no other tool calls unless the command file says otherwise.
4. If `com get <name>` reports that the command does not exist, reply with one line: `Unknown command: $$name. Run $$commands to see what's available.`
5. A bare `$$` is the same as `$$help`.

Only the first token counts: `$$commands please` runs `$$commands` and ignores `please` unless the command takes arguments.

## Adding a command

1. Run `com add <name>` to create `./commands/<name>.md`.
2. Write the command's header (`Usage:`, `Args:`, `Description:`) and execution instructions into `./commands/<name>.md`.
