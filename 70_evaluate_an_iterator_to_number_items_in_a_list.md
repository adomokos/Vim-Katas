### Evaluate an iterator to number items in a list

Change this text:

```shell
partridge in a pear tree
turtle doves
French hens
calling birds
golden rings
```

to:

```shell
1) partridge in a pear tree
2) turtle doves
3) French hens
4) calling birds
5) golden rings
```

Use the expression register to do the loop  
`:let i=1` - set the i var to 1  
`qa` - record the the macro in the 'a' register  
`I<C-r>=i<CR>)<Esc>` - insert the value of i  
`let i += 1` - increment i by 1  
`q` - finish recording the macro  

`:'<,'>norm @a` - execute the macro on the visual selection in parallel
