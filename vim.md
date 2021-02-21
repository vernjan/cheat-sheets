# Vim

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

## Text manipulation
- `x, X` - delete, backspace
- `d<MOVE>`
    - `dw` - delete word
    - `d2W` - delete 2 WORDS
    - `dt"` - delete till `"`
- `dd` - delete line
- `D, d$` - delete until the end of line

## Commands
- `:q[!]` - (force) quit
- `:w [FILENAME]` - save (write) the file
- `:x` or `ZZ` - save the file and exit
- `:e FILENAME` - load (edit) file

## Modes



TODO
---
   
---

ctrl+w switch windows
:e open (edit) file
:ls list opened files (buffers)
:b # go to buffer
:bd close buffer

tab completion
ctrl+d list completion options

---

*,# next/prev word occurence
2G go to line 2

search supports regex

. repeat the commands which change the contents of the buffer


- i (I)
- a (A)
- r (R)


word/WORD


u undo, U undo line
ctrl+R redo
operator [number] motion - operators: d, c, y, ..
registers
buffers
p (P) paste/put
r replace
c change, c$ = C
s substitute
ctrl+g status (filename, line,..)

/ search forward
/foo\c search ignore case
:set hls (hlsearch) - highlight search result (:set nohls)
:set ic (ignorecase) - ignore case (:set noic)
:set is (incsearch) - incremental search (jumps immediatelly)
prepend with 'no' to turn off

? search backward
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


http://iccf-holland.org/click5.html



