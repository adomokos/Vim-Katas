### Paste from register in insert mode

Here is an unfinished excerp of text:

```text
Practical Vim, by Drew Neil
Read Drew Neil's 
```

Copy and paste the page title here:

`yt,` - yanks the text 'Practical Vim  
`jA`  - jumps to the end of the second line  
`<C-r>0` - pastes the text from register  
`.<Esc>` - adds the dot to the very end  

Make it look like this:

```text
Practical Vim, by Drew Neil
Read Drew Neil's Practical Vim.
```
