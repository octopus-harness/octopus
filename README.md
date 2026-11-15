# octopus

Personal reference repo: hand-maintained lists of tools, plus a small `$$` command
protocol for the agent.

## Contents

| File | What it holds |
| --- | --- |
| `cli.md` | Installed CLI / TUI clients |
| `mcps.md` | Installed MCP servers and their tools |
| `COMMANDS.md` | The `$$` command registry |
| `AGENTS.md` | Agent guide and `$$` command protocol |

## Agent commands

In an OpenCode session in this repo, a message that starts with `$$` is a command:

- `$$commands` — list all available commands
- `$$help` — print the help message
- `$$help <command>` — details for one command

See [`COMMANDS.md`](COMMANDS.md) for the full registry.
