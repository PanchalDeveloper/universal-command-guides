# Vim Shortcuts from the Terminal

- `$ vim -o <file_name_1> <file_name_2>` - Open multiple files in Splited Vim buffer tabs (Horizontally)
- `$ vim -O <file_name_1> <file_name_2>` - Open multiple files in Splited Vim buffer tabs (Vertically)
- `$ vim +<line_number> <file_name>` - Open a file named `<file_name>` in a new Vim buffer with the cursor at the line `<line_number>`


# Vim Editor Commands Guide

## Command Mode

- `Esc`: Enter command mode
- `x` or `Del`: Delete a character
- `X`: Delete character in backspace mode
- `u`: Undo changes
- `Ctrl + r`: Redo changes
- `yy`: Copy a line
- `dd`: Delete a line (Also copies the deleted line)
- `D`: Remove a line after cursor
- `p`: Paste the content of the buffer
- `/search_term`: Search for a term
- `n`: Cycle through search matches (forward)
- `N`: Cycle through search matches (backward)
- `[[` or `gg`: Move to the beginning of a file
- `]]` or `G`: Move to the end of a file
- `:%s/foo/bar/gci`: Search and replace all occurrences with confirmation
- `:set number`: Add 'Line Number' column at the start of vim tab
- `:set nonumber`: Remove 'Line Number' column at the start of vim tab

## Insert Mode

- `i`: Enter insert mode

## Visual Mode

- `v`: Start visual mode
- `V`: Start linewise visual mode
- `Ctrl + v`: Start blockwise visual mode

## Saving and Exiting

- `:w`: Save changes
- `:wq` or `ZZ`: Save and quit Vim
- `:q!`: Force quit Vim discarding all changes

## Advanced Vim Commands

### Selecting Lines

- `:m,n` - Select lines from line number `m` to `n`

### Copying Selected Lines

- `:'<,'>y` - Yank (copy) the selected lines

### Copying All Text

- `:%y` - Yank (copy) all lines in the file

### Deleting Selected Lines

- `:'<,'>d` - Delete (cut) the selected lines

### Deleting All Text

- `:%d` - Delete (cut) all lines in the file

### Moving Selected Lines

- `:'<,'>m <line_number>` - Move selected lines to after the specified line number

### Storing Commands in a File

- `:enew` - Edit the contents of a New Empty Vim buffer
- `:w <file_name>` - Write the current Vim buffer to a file named `<file_name>`
- `:r <file_name>` - Read the contents of a file named `<file_name>` into the current Vim buffer
- `:e <file_name>` - Add a new Vim buffer with the contents of a file named `<file_name>` and sets it as 'current buffer'
- `:bdadd <file_name>` - Add a new Vim buffer with the contents of a file named `<file_name>` without setting it as 'current buffer'
- `:bp` - Move to Previous Vim buffer
- `:bn` - Move to Next Vim buffer
- `:bd` - Delete the current Vim buffer
- `:split <file_name>` OR `:sp <file_name>` - Split the current file vim tab with a new vim tab with file named `<file_name>` opened in it (Horizontally)
- `:vsplit <file_name>` OR `:vsp <file_name>` OR `:vs <file_name>` - Split the current file vim tab with a new vim tab with file named `<file_name>` opened in it (Vertically)
- `:Ctrl + ww` - Move to next Split vim tab
- `:m,n w <file_name>` - Write lines `m` to `n` to a file named `<file_name>`
- `:m,n w >> <file_name>` - Append lines `m` to `n` to the end of a file named `<file_name>`

### Saving All Text to Another File

- `:%w <file_name>` - Write the entire buffer to a new file named `<file_name>`
- `:%w >> <file_name>` - Append the entire buffer to the end of an existing file named `<file_name>`
