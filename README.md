# octopus

Personal reference repo: hand-maintained lists of tools, plus a small `$$` command
protocol for the agent. Work happens in the `workspace/` folder.

## Contents

| File | What it holds |
| --- | --- |
| `CLI.md` | the CLI TUI client stack |
| `COMMANDS.md` | The `$$` command registry |
| `AGENTS.md` | Agent guide and `$$` command protocol |
| `workspace/` | Active work folder (not tracked by git) |
| `bin/work` | CLI tool to manage workspace folders and archiving |
| `commands/` | Local command markdown files (not tracked by git) |
| `bin/com` | CLI tool to add and read command docs |

## Agent commands

In an OpenCode session in this repo, a message that starts with `$$` is a command:

- `$$commands` — list all available commands
- `$$help` — print the help message
- `$$help <command>` — details for one command

See [`COMMANDS.md`](COMMANDS.md) for the full registry.
