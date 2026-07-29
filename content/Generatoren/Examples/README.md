# Randomness — example generators

This folder was seeded by the Randomness plugin. Each `.rdm` file
demonstrates a feature or pattern; the numbered prefix is a
suggested reading order.

| File | What it covers |
| --- | --- |
| 01-greetings.rdm | The basics: one table, multiple items |
| 02-tavern.rdm | Tables calling other tables |
| 03-monster.rdm | Variables, prompts, dice, inline tables |
| 04-shop.rdm | Lookup tables (d%), repetitions |
| 05-treasure-dictionary.rdm | Dictionary tables, conditionals |

## How to run them

In any note, add a fenced `randomness` codeblock and roll a
table by name:

```text
```randomness
[@TavernName]
```
```

Click the codeblock to roll. The plugin will find the file
containing the table automatically — you don't need to specify
which file the table lives in.

You can also reference a specific file with `Use:`:

```text
```randomness
Use: 02-tavern.rdm
[@TavernName]
```
```

## Editing the files

These are plain text files. Open them in any editor (Obsidian
itself works) and modify them. Changes take effect immediately;
no reload needed. If you break a file, the codeblock that uses
it will show an error message — fix the file and the error
clears on the next render.

## Removing the examples

Delete the files (or this whole folder) when you don't need them
any more. The plugin won't recreate them; they're a one-shot
seeding for new users.
