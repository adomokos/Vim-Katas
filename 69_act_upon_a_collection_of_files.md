### Act Upon a Collection of Files

`:cd ruby_module` - move into the "ruby_module" dir
`:args *.rb` - open all the .rb files there
`:args` - review all the files

`:first` - move to the first
`:last` - move to the last

Start on the first one
`qa` - record the macro into "a" register
`gg/class<CR>` - find the "class" word
`Omodule Rank` - add the "module Rank" above
`j>G` - indent the file
`Goend<Esc>` - add the "end" to the bottom
`q` - end recording the macro

`:edit!` - undo all edits of the first file
`:argdo normal @a` - run the macro in parallel
