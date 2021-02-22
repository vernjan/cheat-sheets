# Vim

- `u` - undo single change
- `U` - undo all changes on the same line  
- `ctrl+r` - redo
- `ctrl+g` - show status bar (filename, total number of lines, ...)

## Insert mode

### Switch to insert mode
- `i` - insert before cursor
- `I` - insert at the beginning of the line 
- `a` - append after cursor
- `A` - append at the end of the line


## Command mode  
- `ctrl+d` - list completion options 
- `tab` - completion

### Commands
- `:q[!]` - (force) quit
- `:w [FILENAME]` - save (write) the file
- `:x` or `ZZ` - save the file and exit

## Movement
- `h, j, k, l`  - move left, down, up, right
- `w, W` - next word/WORD
- `e, E` - end of this or next word/WORD
- `b, B` - beginning of this or previous word/WORD
- `gg` - first line
- `G` - last line
- `<NUMBER>G` - go to line number
- `0` - start of line
- `^` - start of line after whitespaces
- `$` - end of line
- `*, #` - go to the next (previous) occurrence of this word

## Text manipulation
- `x, X` - delete, backspace
- `d<MOVE>`
    - `dw` - delete word
    - `d2W` - delete 2 WORDS
    - `dt"` - delete till `"`
- `dd` - delete line
- `D, d$` - delete until the end of line
- `.` - repeat the last _manipulation_ command


## Modes
https://www.freecodecamp.org/news/vim-editor-modes-explained/
- normal
- insert
- visual  
- command  
- replace

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

## 

TODO
---
search supports regex
- r (R)
word/WORD
operator [number] motion - operators: d, c, y, ..
registers
p (P) paste/put
r replace
c change, c$ = C
s substitute
/ search forward
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
n, N navigate search
ctrl+o, ctrl+i navigace v historii pohybu vpred/vzad, nutno jeste vyzkouset
% matchin parentheses
Substitute command
:s/old/new - replace once in line
:s/old/new/g - replace all in line
/+c - ask for confirm
:%s - replace in file
:#,#s - replace in line range
ctrl Y, E scrolling up/down, U,D a taky B,f
:! execute external command
VISUAL MODE
v visual
v + w: FILE_PART
move, delete, yank, ..
:r read file into this file
:r !ls read command output into this file (nice)
o, O new line