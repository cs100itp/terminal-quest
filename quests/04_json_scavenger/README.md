# Quest 4 — JSON quote detective

JSON is an example of a _data serialization format_. It is used to store
structured information about objects in a text file.

In `data/quotes.jsonl`, you will find a list of JSON objects (one per line).
Each object has `key`, `text`, and `hash` fields.

If you isolate only those objects whose `key` matches your quest 3 password,
you'll obtain a famous CS-related quote. Track down the source of the quote to
complete this quest!

Write the quote's source (its author's name) in `answers/04_quote_author.txt`
and **commit**.

```
git commit -am "Quest 4: added quote author"
```

Hint: there are plenty of tools that help automate the search and filtering of
JSON data. To select just the `text` fields of those objects whose keys match
YOURKEY from the file FILENAME, you can do:

```
jq -r 'select(.key=="YOURKEY") | .text' FILENAME
```
