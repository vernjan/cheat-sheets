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

### Scrolling
- `gg` - first line
- `G` - last line
- `<NUMBER>G` - go to line number
- `H, M, L` - jump to screen position without scrolling (high, middle, low)
- `ctrl+d, ctrl+u` - scroll half screen down/up
- `ctrl+f, ctrl+b` - scroll full screen front/back
- `ctrl+e, ctrl+y` - scroll one line down/up

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

## Search & Replace
- `/, ?`- search forward/backward (_regex_ supported)
- `n, N` - next/previous search occurrence

## TODO
- operators - d, y, c
- motion numbers - 1, 2, 3, ..
- copy & paste incl.  registers
- text-objects
- external commands (:! ls)

TODO Search & Replace
---
/foo\c search ignore case
:set hls (hlsearch) - highlight search result (:set nohls)
:set ic (ignorecase) - ignore case (:set noic)
:set is (incsearch) - incremental search (jumps immediatelly)
prepend with 'no' to turn off
? search backward
  % Means across all lines
  s Means substitute
  /foo is regex to find things to replace
  /bar/ is regex to replace things with
  /g means global, otherwise it would only execute once per line
j
ctrl+o, ctrl+i navigace v historii pohybu vpred/vzad, nutno jeste vyzkouset
Substitute command
:s/old/new - replace once in line
:s/old/new/g - replace all in line
/+c - ask for confirm
:%s - replace in file
:#,#s - replace in line range
