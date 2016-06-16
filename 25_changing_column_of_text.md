Suppose there is this text:

li.one   a{ background-image: url('/images/sprite.png'); }
li.two   a{ background-image: url('/images/sprite.png'); }
li.three a{ background-image: url('/images/sprite.png'); }

The 'sprite.png' has moved from 'images' to 'components'.

`<C-v>jje` - visual select the entire block
`c` - change the selection
`components` - type in the text 'components'
`<Esc>` - add the word 'components' to the other lines
Note, `<C-c>` is not `<Esc>` :-(

You should see this:

li.one   a{ background-image: url('/components/sprite.png'); }
li.two   a{ background-image: url('/components/sprite.png'); }
li.three a{ background-image: url('/components/sprite.png'); }
