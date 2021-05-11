# IntelliJ IDEA

https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf

## Editing

### Code completion

- `ctrl + space` - basic code completion ✔️
- `ctrl + shift + space` - smart code completion
    - `enter` - insert
    - `tab` - replace
- `ctrl + shift + enter` - complete statement (`cmd + shift + enter`)
- `alt + enter` - show intention actions and quick-fixes ✔️
- `ctrl + F1` - show descriptions of error or warning at caret (`cmd + F1`)
    - `alt + shift + enter` - apply suggested fix

### Code generation
- `alt + insert` - generate code (`cmd + n`)
- `ctrl + alt + t` - surround with (if, else, try, catch, ..) (`cmd + alt + t`)
- `ctrl + o` - override methods
- `ctrl + i` - implement methods
  
### Code info
- `ctrl + p` - parameter info (`cmd + p`)
- `ctrl + mouse` - brief info, resolves `var` type (`cmd + mouse`)
- `ctrl + q` - quick documentation lookup (`cmd + j`, `F1`)
- `alt + q` - context info (current method, class) (`ctrl + shift + q`)

### Text manipulation
- `ctrl + d` - duplicate line (`cmd + d`) ✔️
- `ctrl + y` - delete line (`cmd + backspace`) ✔️
- `ctrl + shift + j` - join lines ✔
- `shift + enter` - start new line (the current line remains unchanged) ✔️
- `ctrl + enter` - new line, don't move the cursor (`cmd + enter`)

- `ctrl + backspace/delete` - delete to word start/end
- `ctrl + shift + backspace/delete` - delete to line start/end 🆕

- `alt + shift + up/down` - swap lines ✔
- `ctrl + shift + up/down` - swap methods/blocks (`cmd + shift + up/down`) ✔

- `ctrl + c` - copy line (`cmd + c`)
- `ctrl + x` - cut line (`cmd + x`)
- `ctrl + shift + v` - paste from recent buffers ("local clipboard history") (`cmd + shift +v`)

- `ctrl + shift + u` - toggle word (selected block) case

### Multi-cursors
- `alt + shift + click` - add new cursors, multi-select
- `alt + shift + g` - move all cursors to line ends
- `ctrl + alt + shift + j` - select all occurrences of the current word and add cursors (`ctrl + cmd + g`)

### Text selection
- `ctrl + w` - extend selection (`alt + up`) ✔️
- `ctrl + shift + w` - shrink selection (`alt + down`) ✔️
  
- `ctrl + shift + [ / ]` - select till code block start/end

- `alt + mouse drag` - column (rectangular) select
- `alt + shift + insert` - column selection mode (`cmd + shift + 8`)

- `alt + shift + drag` - multi-select

### Code formatting
- `ctrl + alt + l` - reformat code (`cmd + alt + l`) ✔
- `ctrl + alt + o` - optimize imports (`ctrl + alt + o`) ✔
- `ctrl + alt + i` - auto-indent line(s) (`ctrl + alt + i`)

### Others
- `ctrl + +/-` - expand/collapse block
- `ctrl + shift + +/-` - expand/collapse all

- `ctrl + /` - comment / uncomment with line comment (`cmd + /`) ✔
- `ctrl + shift + /` - comment / uncomment with block comment (`cmd + alt + /`) ✔

## Usage search

- `alt + f7` - find usages (tool window)
- `ctrl + f7` - highlight usages in file (`cmd + f7`)
    - `f3` - next usage (`cmd + g`)
    - `shift + f3` - previous usage (`cmd + shift + g`)
- `ctrl + alt + f7` - show usages in file (popup) (`cmd + alt + f7`)

## Navigation

- `shift + shift` - search everywhere ✔
  - `/` to limit search for commands
- `ctrl + n` - search class (`cmd + o`) ✔
- `ctrl + shift + n` - search file (`cmd + shift + o`) ✔
- `ctrl + alt + shift + n` - search symbol (`cmd + alt + o`)  
- `ctrl + shift + a` - search action (`cmd + shift + a`)

- `alt + left/right` - go to previous/next tab (`ctrl + left/right`)
- `ctrl + tab` - tab & tool switcher
- `f12` - go to previous tool window
- `escape` - go to editor (from tool window) ✔
- `shift + escape` - hide active (or last active) window ✔
  
- `ctrl + g` - go to line (`cmd + l`) ✔
  
- `ctrl + e` - recent files popup (`cmd + e`)
    - `ctrl + e` - recent edited files
- `ctrl + shift + e` - recent locations popup (`cmd + shift + e`)    
    - `ctrl + shift + e` recent edited locations


- go to declaration (ctrl+click, cmd+b)
- file structure popup (cmd+F12)
- call hierarchy: callers/callees (ctrl+option+h)
- ! switch between class and test class (shift+cmd+t)
- navigate back/forward (cmd+option+left / cmd+option+right)
- type hierarchy (ctrl+h)

F2/shift + F2




`cmd + shift + ]` - next tab
`cmd + shift + [` - previous tab

## General

- run anything (ctrl+ctrl)

- `ctrl + f4` - close active tab (`cmd + w`)

- TODO open Preferences (`cmd + ,`)
- TODO open Project structure (`cmd + ;`)

- TODO new scratch file (`cmd + shift + n`)
- TODO new file, source, diagram, ...  (`cmd + n)`

## Search/Replace

- find (cmd+f)
- global find (shift+cmd+f)
- replace (cmd+r)
- global replace (shift+cmd+r)
- next (cmd+g)
- previous (shift+cmd+g)

## Refactoring

- rename (shift+f6)
- change signature (cmd+F6)

## Compile and Run

- Run current context (cmd+shift+r)
- Re-run (ctrl+r)

## VCS/Local History

- commit project to VCS (cmd+k)
- push to Git (shift+cmd+k)
- update project from VCS (cmd+t)
- commit window (cmd+0)
- rollback changes (cmd+option+z)
- commit message history (ctrl+m)

## Tool windows

- 0 commit (changelist)
- cmd+k commit (commit message)
- 1 project
- 3 find
- 4 run
- 7 structure

## Others

- compare (cmd+d)
- expand (cmd++)
- collapse (cmd+-)
- refresh (cmd+r)
- next/previous issue (f2/shift+f2)
- new scratch file (shift+cmd+n)
- quick documentation (f1 / ctrl+j)

ctrl + tab