### Tune the case sensitivity of search patterns

Here is a small text snippet to search on:

```
foo
foo & foo
foo & Foo
FOO & foo
```

Setting case sensitivity per search:  
`/foo` - Search for the word "foo"  
`/foo\C` - Search for the word "foo", case sensitive  
`/foo\c` - Search for the word "foo", case insensitive  

`set smartcase` - cancels out of case insensitive search when first upper-cased character is typed
