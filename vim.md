# Vim

- `u` - undo single change
- `U` - undo all changes on the same line  
- `ctrl+r` - redo
- `ctrl+g` - show status bar (filename, total number of lines, ...)

## Insert mode

### Switch to insert mode
- `i` - insert before cursor
- `I` - insert at the beginning of this line 
- `a` - append after cursor
- `A` - append at the end of this line

## Command mode  
- `ctrl+d` - list completion options 
- `tab` - completion

### Commands
- `:q[!]` - (force) quit
- `:w [FILENAME]` - save (write) the file
- `:x` or `ZZ` - save the file and exit
- `:r <FILENAME>` - read an external file into this file
- `:r !<COMMAND>` read external command output into this file (e.g. `:r !ls`)
- `:<NUMBER>` - go to line

## Navigation
- `h, j, k, l`  - left, down, up, right
- `w, W` - next word/WORD
- `e, E` - end of this or next word/WORD
- `b, B` - beginning of this or previous word/WORD
- `ge, gE` - end of previous word/WORD 
- `0` - start of line
- `^` - start of line after whitespaces
- `$` - end of line
- `%` - matching bracket (`(), [], {}`)  
- `*, #` - next (previous) occurrence of this word
- `), (` - next (previous) sentence
- `}, {` - next (previous) paragraph (empty line)
- `]m, [m` - next (previous) start of method (_coding_)
- `]M, [M` - next (previous) end of method (_coding_)
- `[(, ])` - next `(` / previous `)`
- `[{, ]}` - next `}` / previous `{`
- `<NUMBER>|` - jump to column

### Scrolling
- `gg` - first line
- `G` - last line
- `<NUMBER>G` - go to line number
- `H, M, L` - jump to screen position without scrolling (high, middle, low)
- `ctrl+d, ctrl+u` - scroll half screen down/up
- `ctrl+f, ctrl+b` - scroll full screen front/back
- `ctrl+e, ctrl+y` - scroll one line down/up
- `zt, zb, zz` - scroll top, bottom, middle (cursor does not move)

### word vs. WORD
_This is mind-blowing example!_
- **words** - `This`, `is`, `mind`, `-`, `blowing`, `example`, `!`
- **WORDS** - Separated by whitespaces: `This`, `is`, `mind-blowing`, `example!` 

## Text manipulation
- `x, X` - delete, backspace
- `r` - replace single character (`R` enters _replace_ mode)
- `d<MOVE>` - deletion
    - `dw` - delete word
    - `d2W` - delete 2 WORDS
    - `dt"` - delete till `"`
    - `dd` - delete line
    - `d$, D` - delete until the end of this line
- `c<MOVE>` - change (delete and enter _insert_ mode)
    - `c$, C` - change until the end of this line  
- `s` - substitute (delete character and enter _insert_ mode)
- `S, cc` - substitute line (delete line and enter _insert_ mode)
- `o, O` - insert new line after (before) cursor  
- `.` - repeat the last _manipulation_ command
- `~` - change case (upper/lower)
- `J` - join lines


## Modes
https://www.freecodecamp.org/news/vim-editor-modes-explained/
- normal
- insert
- visual  
- command  
- replace

### Visual mode
- `v` - enter _visual_ mode
- `ctrl+v` - enter column _visual_ mode
- `:w <FILENAME>` - write highlighted part into the file

## Viewports
- `:sp[lit]` - split horizontally
- `:vsp[list]` - split vertically  
- `ctrl+w <MOVE>` - switch between windows
  - `ctrl+w h,j,k,l` - switch to window in direction
  - `ctrl+w ctrl+w` - switch to the next window
  - `ctrl+w q` - close window

## Buffers
- `:e FILENAME` - load (edit) file (creates new buffer)
- `:ls` - list buffers
- `:b <NUMBER/NAME>` - switch to buffer by number or name
- `:b #` - switch to previous buffer   
- `:bd` - close buffer

## Copy & Paste
- `p, P` - paste after/before line (cursor)
- `y<MOVE>` - copy (yank) 
- `"<REGISTER_NAME>` - copy into / paste from the specific registers
- `"<CAPITAL_REGISTER_NAME>y<MOVE>` - append into register

### Registers
_Whatever is deleted or copied (yanked) goes into registers._
- `:reg` - show registers

### Types of registers
- _line (l)_ vs. _character (c)_
- `""` - default register
- `"0-9` - numbered registers - history
- `"a-z` - custom named registers
  - `"ay$` - copy from the current cursor position until the end of line into register `a`
  - `"ap` - paste from register `a`  
- `"-` - small register holds last _character-wise_ yank/delete
- `"_` - black hole register (like `/dev/null`)
- `"/` - last search register

## Search & Replace
- `/, ?` - search forward/backward (supports _regex_)
  - `/foo\c` - case in-sensitive
  - `/foo\C` - case-sensitive
- `n, N` - next/previous search result

### Configuration
- `:set hls` - (`hlsearch`) - highlight search results
- `:set ic` - (`ignorecase`) - ignore case
- `:set is` - (`incsearch`) - incremental search (jump immediately to results)

### Tips
- Pressing `/` (or `?`) + `enter` repeats the last search


### Replacing
https://linuxize.com/post/vim-find-replace/
```
:[range]s/{pattern}/{string}/[flags] [count]
```

- `:s/pattern/string` - replace once on this line (use empty _string_ for deletion)
- `:%s/pattern/string` - replace once/all (based on setting) in this buffer (file)
- `:#,#s/pattern/string` - replace in line range
  - `:3,10s/foo/bar/g` - replace from 3rd to 10th line 
  - `:.,$s/foo/bar/` - replace from the current line till the end of buffer
  - `:.,+4s/foo/bar/g` - replace till 4 lines below the current line

### Flags
- `g` - global - replace all in the given context (line, range, buffer)
- `c` - ask for confirmation
- `i` - case in-sensitive (you can also use `:s/pattern\c/string`)
- `I` - case-sensitive (you can also use `:s/pattern\C/string`)

## TODO
- operators - d, y, c
- motion numbers - 1, 2, 3, ..
- text-objects
- external commands (:! ls)
- marks: `m`, ```, `'`, :marks, :delm [!]
- advanced moves
  - `d/foo` - delete until foo
  - `4/foo` - find 4th foo
- overAll organization  
