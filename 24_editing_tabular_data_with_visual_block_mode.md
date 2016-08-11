### Editing tabular data with visual block mode

```
Chapter             Page
Normal Mode           15
Insert Mode           31
Visual Mode           44
```

Make it look like this

```
Chapter      | Page
-------------------
Normal Mode  |   15
Insert Mode  |   31
Visual Mode  |   44
```

`<C-v>3j` - block select the column to the point we need to delete back  
`d...` - delete the columns  
`gv` - reselects the same visual selection  
`r|` - repeats adding the pipe  
`yy` - duplicate the first row  
`Vr-` - select the entire line, repeat the "-" for the row  
