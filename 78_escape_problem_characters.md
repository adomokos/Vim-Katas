### Escape Problem Characters

```text
Search items: [http://vimdoc.net/search?q=/\\][s]
...
[s]: http://vimdoc.net/search?q=/\\
```

`"uyi[` - yank the url into register 'u'  
`/\V<C-r>u<CR>` - to populate the search field  

We could escape the backslash, but that's tedious.

Vim will search forward with `/` character, but with `?` it searches backwards.  

`?http://vimdoc.net/search?q=/\\` - will match everything until the '?'  
