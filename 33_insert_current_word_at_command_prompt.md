Rename the variable 'tally' to 'counter':

var tally;
for (counter=1; tally <= 10; tally++) {
  // Do something with tally
};

Start on line 3 at the 't' character
`*` - selects all the words 'tally'
`cwcounter<Esc>` - replaces the word with counter
`:%s//<C-r><C-w>/g` - gets the current word for the
substitute command
