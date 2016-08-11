### Append after a ragged visual block

We already had this text before:

```javascript
var foo = 1
var bar = 'a'
var foobar = foo + bar
````

Append ';' at the end of each line using visual mode.

Start on the first line, at "1"  
`<C-v>jj$`  
`A;` - appends the ';' at the end of each line  
`<Esc>` - will apply it for each selected line  
