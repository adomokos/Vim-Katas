### Duplicate or move lines

Given this text:

```
Shopping list
    Hardware store
        Buy new hammer
    Beauty parlor
        Buy nail polish remover
        Buy nails
```

Do the following exercises on the text above:

Start at 'H' on line 6  
`:8copy.` - copies line to current line  
`:8t.` - should do the same  
`:t.` - duplicate current line  
`:t$` - copy current line to end of file  

`:8m$` - move line 8 to the end of the file  
Visual select 2 lines  
`:'<,'>m$` move the selected lines to the end of the file  
