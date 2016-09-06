### Stake the boundaries of a word

```
the problem with these new recruits is that
they don't keep their boots clean.
```

`/the` - will yield results with words where "the" is embedded, like "they"  
`/\v<the>` - will find only the exact macthes  

The `<` and `>` are zero-width items, they represent boundaries.

`/\<the\>` - will match the angle brackets as chars  


