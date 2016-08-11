### Edit the contents of a macro

```text
1. One
2. Two
3. three
4. four
```

Some of the lines use capital letter, `~` would just switch casing, we need to use `vU` here, which makes the char upper-cased at the cursor.

This is what is should look like after your changes:

```test
1) One
2) Two
3) Three
4) Four
```

`:put a` - paste the content of register a into the doc  
Edit the macro by replacing `~` with `vU`  
Remove the last J, as it will be added back  
`"add` - replaces the current line with register a  

Characterwise yank is a safer bet, try this instead:  
`0` - go back to the first char in line  
`"ay$` - yank the content of the line  
`dd` - delete the line  
