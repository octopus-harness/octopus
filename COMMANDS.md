# $$ Commands

Messages that begin with `$$` run the matching command from `./commands`.

## Using `com`

Use the `com` CLI tool to manage and read command definitions:

* Read a command: `com get <name>` (prints `./commands/<name>.md`)
* Create a command: `com add <name>` (creates `./commands/<name>.md`)
* Interactive mode: `com` (prompts for `add` or `get` and lets you pick a file)
* Help: `com help`

Strip the leading `$$` before passing `<name>` to `com` (for example, `$$help` maps to `com get help`).

## Command File Format

Every command file in `./commands/<name>.md` starts with a three-line header followed by its execution instructions:

```text
Usage: $$<name> [args]
Args: <args or "-">
Description: <one-line summary>
```

## Running a Command

1. Parse `$$name [args...]` from the start of the message (case-insensitive). A bare `$$` runs `$$help`.
2. Run `com get <name>` to load the command definition.
3. If `com get <name>` fails because the command file does not exist, reply with one line: `Unknown command: $$name. Run $$commands to see what's available.`
4. Follow the loaded instructions cleanly: no preamble, no trailing commentary, and no file edits unless the command specifies otherwise.
