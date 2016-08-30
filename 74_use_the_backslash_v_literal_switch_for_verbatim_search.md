### Use the \v literal switch for verbatim search

Use this excerpt of text:

```
The N key searches backwards...
... the \v pattern swtich (a.k.a. very magic search)...
```

`/a.k.a.` - will match more than 1 result
`/a\.k\.a\.` - will find the right word, but escaping the dots is a lot of work
`/\Va.k.a.` - turns off all special char in regex, only backslash is escaped

General rule:  
If you search for a regular expression use the `\v`, if you want to search for
verbatim text, use the `\V` switch.

