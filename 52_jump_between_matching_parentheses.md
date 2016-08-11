### Jump between matching parentheses

Let's say there is this console statement:

```javascript
console.log([{'a':1},{'b':2}]);
```

Start on the first opening paren  
`%` - jumps to the closing paren  
`h` - select the last ']' bracket  
`%` - jump to the first '[' bracket  
`l` - select the first curly '{'  
`%` - jump to the last curly  

```ruby
%w{London Berlin New\ York}
```

`dt{` - deletes the '%w' part  
`%` - jumps to the closing curly  
`r]` - replace curly with square bracket  
`tick tick` - jumps to the first curly  
`r[` - replaces the opening curly with square bracket  
