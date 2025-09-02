# Quest 2 — Decode the hidden password

We often encounter _binary files_ which mostly consist of illegible data, but
which may contain useful nuggets of information. `data/blob.bin` is such a file,
from which you are to extract strings which you will attempt to decode based on
a popular data encoding format: base64. There are many decoys! Only one string
will decode to a sensible word, which will be both the answer for this quest and
the password for the next.

## Hints

To extract usable strings from a binary file named FILENAME, do:

```
strings FILENAME
```

Try decoding a string as base64 with:

```
echo "the-base64-string" | base64 -d
```

When you find it, write the decoded password into `answers/02_password.txt`,
then **commit**:

```
git commit -am "Quest 2: added password from binary"
```
