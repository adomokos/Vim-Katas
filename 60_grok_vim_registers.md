### Grok Vim registers

Given this text

```text
1) This is the first block of text
2) Another block of text
```

`"ayy` - will yank the first line into register "a"  
`"byy` - yank the 2nd line into register "b"  
`"bp` - paste in from register "b" first  
`"ap` - paste in from register "a" after  

Use the yank register to fix the text from previous kata

```javascript
collection = getCollection();
process(somethingInTheWay, target);
```

`yiw` - to yank the word into yank register  
`jww` - to go to next line to the beginning of "somethingInTheWay"  
`dw` - will delete the word  
`"0P` - will insert the word from the yank register  

`:reg "0` - will inspect the yank and unnamed registers

`"_` - is the black hole register, nothing returns from there

`"+` - system clip board  
`"*` - system selection  

Visual select this entire doc, yank its content into `"+yy`, go to
Pages and insert it into a new document there

`"=` - expressions register

`i` - switch to insert mode  
`<C-r>=` - switches to expression register  
`6*35<CR>` - will provide the text "210" and drop back into insert mode  

## More registers
`<C-r>%` - name of the current file  
`<C-r>#` - name of the alternate file  
`<C-r>.` - last inserted text  
