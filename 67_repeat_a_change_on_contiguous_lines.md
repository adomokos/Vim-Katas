### Repeat a Change on Contiguous Lines

Given this text:
```
1. one
2. two
3. three
4. four
5. five
```

Change it to be like this:
```
1) One
2) Two
3) Three
4) Four
5) Five
```

`qa` - record the macro in the "a" register  
`0f.` - find the dot on the first line  
`r)` - replace the dot with a ")"  
`w~` - title-case the word  
`j` - move down 1 line  
`q` - quit recording the macro  

We can replay the macro with this:  
`@a` - and `@@` after that  

But what if there is line barrier in the text like this?
```
1. one
2. two
3. three
// Some comment
4. four
5. five
```

Replay it with the highlighted text:  
`'<,'>norm @a` - this will replay the macro from the "a" register on the highlighted lines  
