### Snap between files using global marks

While `m{a-z}` sets a local mark in the current file  
`m{A-Z}` - sets a global mark  

`vs 01_` - open the 01_ markdown file  
`:10` - go to the 10th line  
`mA` - mark the position there  
switch back to this file  
`backticA` - takes you back to the file's location  

`:vimgrep /cursor/ **` - searches for the word in the current dir,  
  takes you there  
`:cn` - takes you to next result  
`:cp` - take you to previous result  
