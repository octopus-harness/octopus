# $$ Commands

Messages that begin with `$$` run the matching command from this file. Rows are listed in display order; `$$commands` prints them in this order.

## Index

| Command | Args | Description |
| --- | --- | --- |
| `$$commands` | — | List all available commands |
| `$$help` | `[command]` | Show the help message, or details for one command |

## $$commands

Usage: `$$commands`

Reply with the line `2 commands available:` followed by a Markdown table with the columns
`Command`, `Args` and `Description`, copied from the index above in the same order.
Nothing before or after it.

## $$help

Usage: `$$help [command]`

**Without an argument**, print this help message:

```text
`$$` commands — a message that begins with `$$` runs the matching command.

Usage: $$<command> [args]

Commands:
  $$commands        List all available commands
  $$help            Show the help message, or details for one command
  $$help <command>  Show details for one command

Example: $$help $$commands

Add or change commands in COMMANDS.md.
```

**With an argument**, strip a leading `$$` from the argument and match it case-insensitively
against the index:

- If it matches, print that command's section (usage, arguments, example) on its own,
  without the rest of the commands.
- If it doesn't match, reply with one line: `Unknown command: <arg>. Run $$commands to see what's available.`
