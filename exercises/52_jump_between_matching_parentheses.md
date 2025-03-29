### Jump between matching parentheses

Let's say there is this console statement:

```javascript
console.log([{'a':1},{'b':2}]);
```

`f(` - forward to the first '('
`%` - jump to the closing ')'
`h` - move left - to the last ']' bracket
`%` - jump to the first '[' bracket
`l` - move right - to the first curly '{'
`%` - jump to the matching curly '}'

```ruby
%w{London Berlin New\ York}
```

`dt{` - delete the '%w' part
`%` - jump to the closing curly bracket
`r]` - replace '}' with ']'
`''` or `backtick backtick` (\`\`) - go to the position before the last jump, i.e. the location of the first curly bracket
`r[` - replace '{' with ']'
