### Operate with a search motion

Given this text, delete the part "takes time but eventually".

```
This phrase takes time but
eventually gets to the point.
```

`/ta<CR>` - move the cursor to the beginning of the word "takes"
`v` - enter into character-wise visual mode
`/ge<CR>` - highlight 'til the word 'gets'
`h` - moves back 1 char
`d` - deletes the content

Here is a quicker way of doing the same thing:

`d/ge<CR>` - does the whole thing in 1 move
