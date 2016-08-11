### Use count

Change this text:

```css
.blog, .news { background-image: url(/sprite.png); }
.blog { background-position: 0px 0px }
```

to this:

```css
.blog, .news { background-image: url(/sprite.png); }
.blog, .news { background-image: url(/sprite.png); }
.news { background-position: -180px 0px }
```

Moves:

1. `yyp` to duplicate the last line  
2. `cW.news<Esc>` to replace the word 'blog' with 'news'  
3. `180<C-x>`  
