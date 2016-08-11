### Overwrite existing text

Example text:

```text
Typing in insert mode extends the line. But in replace mode
the line length does not change.
```

Change the ". But" to ", but" in replace mode

`f.` - find the dot  
`R, b<Esc>` - enter into replace mode, replace . with comma, space and replace "B" with "b"  

`gR` triggers the Virtual Replace Mode, which is better, as that handles the tab spaces.
