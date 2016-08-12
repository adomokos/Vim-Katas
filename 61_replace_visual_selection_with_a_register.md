### Replace visual selection with a register

There is an easier way to swap the word "somethingInTheWay" with "collection"

```javascript
collection = getCollection();
process(somethingInTheWay, target);
```

`yiw` - to yank the word into the yank register  
`jww` - to move to 's' char in "somethingInTheWay"  
`ve` - visually selects the entire word  
`p` - will insert the yanked word over the visually selected text  

Another exercise: swap the 2 words "chips" and "fish"

I like chips and fish.

Start on 'I'  
`fc` - find the first word to swap  
`de` - delete the word  
`mm` - mark the place  
`ww` - move to 'f' in "fish"  
`ve` - visually select the word  
`p` - paste the word over "fish"  
`backtickm` - to take back to the mark position  
`P` - to insert the word fish  
