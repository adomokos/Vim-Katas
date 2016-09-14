### Operate on complete search match

Make this:

```ruby
class XhtmlDocument < XmlDocument; end
class XhtmlTag < XmlTag; end
```
to be like this:

```ruby
class XHTMLDocument < XMLDocument; end
class XHTMLTag < XMLTag; end
```

One possible solution:  
`/\vX(ht)?ml\C<CR>` - find the items to change  
`gU//e<CR>` - make the text uppercase - we use '//e' as a motion  
`//<CR>` - move to next item  
`.` - rerun the command  
`//<CR>.` - move to next item and rerun the command  
