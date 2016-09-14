### Offset cursor to the end of a search match

Use this text as an example:

```text
Aim to learn a new programming lang each year.
Which lang did you pick up last year?
Which langs would you like to learn?
```

Task: replace "lang" with "language".

`{start} on A of Aim` - initial position  
`/lang/e<CR>` - find the word 'lang'  
`auage<Esc>` - add "uage" to "lang"  
`n.n.` - repeat it twice  
