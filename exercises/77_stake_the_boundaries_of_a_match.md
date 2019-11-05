### Stake the boundaries of a match

Sometimes we might want to specify a broad pattern, then focus on a subset
of that match. Vim's `\zs` and `\ze` items allow just to do that.

```text
Practical Vim is really a great book.
```

`/Practical Vim<CR>` - will match the word "Practical Vim"
`/Practical \zsVim<CR>` - will match the "Vim" from the maches

```test
Match "quoted words" not quote marks.
```

`/\v"[^"]+"` - matches the word with quotes (`[^"]+` - match anything that's not a quote mark)
`/\v"\zs[^"]+\ze"` - matches words inside the quote

