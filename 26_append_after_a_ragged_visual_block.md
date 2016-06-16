We already had this text before:

var foo = 1;
var bar = 'a';
var foobar = foo + bar;

Append ';' at the end of each line using visual mode.

`<C-v>jj$`
`A;` - appends the ';' at the end of each line
`<Esc>` - will apply it for each selected line
