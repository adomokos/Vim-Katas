###  Create complex patterns by iterating upon search history

Change the single quotes to double quotes.

```
This string contains a "quoted" word.
This string contains "two" quoted "words".
This "string doesn't make things easy".
```

`/\v".+"` - will match everything in single quote, quote included  
`/<Up>` - Use search history get this search string back  
`/\v"[^"]+` - this will be better, but not perfect   
Use search history again  
`/\v"([^"]|"\w])+"` - this should be an even better match  
`q/` - let's use the search command-line window  
Find this search: `/\v"[^"]+` - to edit  
`f[` - jump to the first square bracket  
`c%(<C-r>")<Esc>` - cut and paste + insert parens  
`i|'\w<Esc>` - inserts the remaining search  

We want to capture everything in the quotes, wrap it in parens  
`/\v'(([^']|'\w)+)'` - this is perfect
`:%s//'\1'/g` - replace double quotes with single quotes by using a %1 capture register  
