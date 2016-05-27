Change the text below to look like this
(please notice the added spaces around "+")

var foo = "method(" + argument1 + "," + argument2 + ")";

Steps:
1. find "+" with `f+`
2. delete and switch to insert mode with `s`
3. Type ` + `
4. Leave insert mode
5. find the next "+" with `;`
6. Repeat with `.`

var foo = "method("+argument1+","+argument2+")";
