### Exec commands on one or more consecutive lines

Look at this HTML sample:

```html
<!DOCTYPE html>
<html>
  <head><title>Practical Vim</title></head>
  <body>
    <h1>Practical Vim</h1>
  </body>
</html>
```

Do the following exercises on the text avove:

`:3` - move to line 3  
`:print` print current line  
`:5p` - move to line 5, print it  
`:6d` - move to line 6 and delete it in 1 command  
`:3,5p` - print range  
`:.,$p` - print from current line ('.') to the end ('$')  
`:%p` - % means the entire file  
visual select multiple lines, `:'<,'>p` - prints the visual selection  
`:/<html>/,/<\/html>/p` - print out everything within html  
`:/<html>/+1,/<\/html>/-1p` - without the html tags  
