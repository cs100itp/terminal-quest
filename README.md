# Terminal Quests

## Goals

After completing this lab, you should be able to use the command line to:

- Navigate between directories and list their contents
- Examine both text and binary files
- Decode/Decrypt different types of data encoding
- Extract information from a JSON file
- Commit your changes to a Git version control repository

## Instructions

This lab takes the form of four "quests", each of which will require you to do a
bit of work on the course server (via the command line. After each step, you
will need to _commit_ your work. Some quests will net you a password that will
be required to start the next one.

Have fun!

## Getting started and looking around

Each quest has its own short writeup -- you can find the writeups underneath the
"quests" directory --- each numbered subdirectory contains a "README.md" file
which you can view by typing `bat README.md` (remember to type `q` to exit the
`bat` viewer).

Some of the quests will reference one or more data files, which you can find in
the "data" directory. Your answers for the quests will all go into files found
in the "answers" directory. After adding your answer to a given file, you should
_commit_ your work with the command:

```bash
git commit -am "Quest N: <what you did>"
```

## Quest summary

1. **Identity card** — Edit a file with your name and ID. Commit.
2. **Hidden password** — Use `strings` on a binary to spot a **single-line**
   "base64" token (there are decoys!). Decode; save the password. Commit.
3. **Decryption** — Use GPG with the quest 2 password to decrypt row,col
   coordinates. Use those to pick characters from `data/romeo.txt`, which spell
   the next password. Commit.
4. **JSON scavenger** — Use the quest 3 password as the `key` to filter JSON
   objects in `data/quotes.jsonl`; concatenate their `text` to read a famous
   quote. Find the author and save their name. Commit.

## Verifying your work

At any point you can review all the commits and corresponding changes you made
to your version control repository with the following command:

```
git log -p
```
