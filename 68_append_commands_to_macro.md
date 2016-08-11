### Append Command to Macro

Let's say we recorded this macro:

```text
1. one
2. two
3. three
4. four
```

`qa` - record in "a" register  
`0f.r)w~` - replace "." with ")" and tile-case word  
`q` - quit recording macro  

We forgot adding the "j" to move to the next line.

Inspect what got recorded:

`:reg a` - look at what's in "a" register

`qA` - append to the macro recorded in "a" register  
`j` - move to next line  
`q` - quit recording the macro  

Look at it again, you should have the "j" at the end
