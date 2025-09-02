# Quest 3 — Decrypting Romeo

Using the password from the previous quest, you can now decrypt the file
`data/coords.encrypted`.

To decrypt the file FILENAME, do:

```
gpg --no-symkey-cache -d FILENAME
```

Note that this will ask you to type in the password interactively. On success,
you will obtain a list of coordinates, which, in conjuction with the famous
soliloquy from "Romeo and Juliet" (found in `data/romeo.txt`), you can use to
deduce the final password.

Can you figure out the password?

Hint: you may want to check out the character positions as reported by a better
editor (try `vi romeo.txt` --- to exit the text editor, hit the escape key then
type the sequence ":q!" and hit enter).

When you have the password, write it to `answers/03_password2.txt`, then
**commit**:

```
git commit -am "Quest 3: added password from Romeo "
```
