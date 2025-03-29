### Paste from register in insert mode

Here is an unfinished excerpt of text:

```text
Practical Vim, by Drew Neil
Read Drew Neil's
```

Copy and paste the page title here:

`yt,` - yanks the text 'Practical Vim
`j` - move to the second line
`A ` - go to the end of line, switch to insert mode and add a space
`<C-r>0` - pastes the text from register
`.<Esc>` - adds the dot to the very end

Make it look like this:

```text
Practical Vim, by Drew Neil
Read Drew Neil's Practical Vim.
```
