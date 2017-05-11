# egghead-learn-vim
Egghead course to learn to use vim text editor.

## Commands
`:q` or `:quit` to exit vim
`:j` to move down a file
`:k` to move up a file
`:l` to move rigth a file
`:h` to move left a file
`:w` to move right word by word a file
`:b` to move left word by word a file 
`:w` or `:write` to save a file, if the file is a new file then it's necessasry supply a name to the command

### Modes:
- Command mode: press `shift + :` here we can issue any commands we want to the editor
- Normal mode: when vim starts, this is where we can navigate around a file using our navigations keys and manipulate text
- Insert mode: press `i` to insert text in the file, to exit from this mode press `Esc` and you return to normal mode
- Visual mode: select blocks of text from the file, press `v`, use movement keys to select text, press `shift + v` to select all line, `Esc` to exit

### Built-in commands
`dd` delete line
`shift + d` delete from the current position until the end of the line
`d` delete the selected text
`cw` delete the current word and enter to insert mode
`d5w` delete five words
`c3j` cut 3 lines down and put into insert mode

### Combining commands
The basic rule to combine commands into Vim it's the order:
- Action
- Location
- Context (second location)

`dw` delete one word
`cw` change (copy) one word and put into insert mode
`cit` copy content and be put right into insert modei
`ci{` copy content inside curly brackets `{ }`
`ci"` copy content inside quote marks `" "`

### Copy and Pastei
Note: the copied text does not get added to the system clipboard

1. `v` to enter visual mode and select text
2. `y` to copy the selected text
3. `p` to paste the copied text

1. `dd` to delete the current line
2. `p` paste the deleted text

1. `dw` delete one word
2. `p` paste the deleted word
