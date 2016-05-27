Chapter             Page
Normal Mode           15
Insert Mode           31
Visual Mode           44

# Make it look like this
<C-v>3j
d..
gv   # reselects the same visual selection
r|   # repeats adding the pipe
yy   # Duplicate the first row
Vr-  # select the entire line, repeat the - for the row

Chapter      | Page
-------------------
Normal Mode  |   15
Insert Mode  |   31
Visual Mode  |   44
