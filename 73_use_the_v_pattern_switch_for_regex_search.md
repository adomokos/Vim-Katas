### Use the \v pattern switch for regex search

Let's use this snippet of CSS:

```css
body   { color: #3c3c3c; }
a      { color: #0000EE; }
strong { color: #000; }
```

`/#\([0-9a-fA-F]\{6}\|[0-9a-fA-F]\{3\}\)` - this regex will match all the hex values

The `\v` switch make Vim's regex search like Perl, Python and Ruby.

`/\v#([0-9a-fA-F]{6}|[0-9a-fA-F]{3})` - the search works the same way, but it does not need to escape the special characters.  
`/\v#(\x{6}|\x{3})` - will be the same as above, but it's using `\x` character class  
`
