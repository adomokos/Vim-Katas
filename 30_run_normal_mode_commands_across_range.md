### Run normal mode commands across range

There is a block of text like this:

```javascript
var foo = 1
var bar = 'a'
var baz = 'z'
var foobar = foo + bar
var foobarbaz = foo + bar + baz
```

`A;<Esc>` - Add semicolon to the end of first line  
Visual select the rows  
`:'<,'>normal.` - repeats the command for all highlighted lines  

or solve it like this:  
`:'<,'>normal A;` - executes normal command for all highlighted lines  

Add semi-colon to all lines in file:  
`:%normal A;`  

Comment out an entire JS file:  
`:%normal i//`  
