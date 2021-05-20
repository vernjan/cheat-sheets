# IntelliJ IDEA

https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf

## Edit

### Text selection
- `ctrl + w` - extend selection (`alt + up`) ✔️
- `ctrl + shift + w` - shrink selection (`alt + down`) ✔️
- `ctrl + shift + [ / ]` - select till code block start/end ⚡
- `alt + mouse drag` - column (rectangular) select ⚡
- `alt + shift + insert` - column selection mode (`cmd + shift + 8`) ✔️

### Text manipulation
- `ctrl + d` - duplicate line (`cmd + d`) ✔️
- `ctrl + y` - delete line (`cmd + backspace`) ✔️
- `ctrl + shift + j` - join lines ✔
- `shift + enter` - start new line (the current line remains unchanged) ✔️
- `ctrl + enter` - new line, don't move the cursor (`cmd + enter`)
- `ctrl + backspace/delete` - delete to word start/end ⚡
- `ctrl + shift + backspace/delete` - delete to line start/end ⭐
- `alt + shift + up/down` - swap lines ✔
- `ctrl + c` - copy line (`cmd + c`) ✔️
- `ctrl + x` - cut line (`cmd + x`) ✔️
- `ctrl + shift + v` - paste from recent buffers ("local clipboard history") (`cmd + shift + v`)
- `ctrl + shift + u` - toggle word (selected block) case ✔️

### Multi-cursors
- `alt + shift + click` - add new cursors, multi-select ⚡
- `alt + shift + drag` - multi-select
- `alt + shift + g` - move all cursors to line ends ⚡
- `ctrl + alt + shift + j` - select all occurrences of the current word and add cursors (`ctrl + cmd + g`) ⚡

## Code

### Code completion
- `ctrl + space` - basic code completion ✔️
- `ctrl + shift + space` - smart code completion
    - `enter` - insert
    - `tab` - replace
- `ctrl + shift + enter` - complete statement (`cmd + shift + enter`) ⚡
- `alt + enter` - show intention actions and quick-fixes ✔️
- `ctrl + F1` - show descriptions of error or warning at caret (`cmd + F1`)
    - `alt + shift + enter` - apply suggested fix

### Code generation
- `alt + insert` - generate code (`cmd + n`) ⚡
- `ctrl + alt + t` - surround with (if, else, try, catch, ..) (`cmd + alt + t`) ⚡
- `ctrl + o` - override methods
- `ctrl + i` - implement methods
  
### Context info
- `ctrl + p` - parameter info (`cmd + p`) ⚡
- `ctrl + mouse` - brief info, resolves `var` type (`cmd + mouse`)
- `ctrl + q` - quick documentation lookup (`ctrl + j`, `F1`)
- `alt + q` - context info (current method, class) (`ctrl + shift + q`)
- `ctrl + shift + p` - expression type info ⚡
- `ctrl + shift + i` - quick definition (`alt + space`)

### Formatting
- `ctrl + alt + l` - reformat code (`cmd + alt + l`) ✔
- `ctrl + alt + o` - optimize imports (`ctrl + alt + o`) ✔
- `ctrl + alt + i` - auto-indent line(s) (`ctrl + alt + i`)

### Editing
- `ctrl + /` - comment / uncomment with line comment (`cmd + /`) ✔
- `ctrl + shift + /` - comment / uncomment with block comment (`cmd + alt + /`) ✔
- `ctrl + shift + up/down` - swap methods/blocks (`cmd + shift + up/down`) ✔

## Navigation
- `ctrl + b / ctrl + click` - go to declaration ✔
- `ctrl + shift + b` - go to type declaration ⚡
- `ctrl + alt + b` - go to implementations (`cmd + shift + b`) ⚡
- `ctrl + u` - go to super class/method (`cmd + u`) ⚡
- `alt + space` - quick definition lookup
- `ctrl + +/-` - expand/collapse block ⚡
- `ctrl + shift + +/-` - expand/collapse all

### Searching
- `shift + shift` - search everywhere ✔
    - `/` - limit search for commands
    - `/url/` - limit search for URL mappings (web endpoints) ⚡
- `ctrl + n` - search class (`cmd + o`) ✔
- `ctrl + shift + n` - search file (`cmd + shift + o`) ✔
- `ctrl + alt + shift + n` - search symbol (`cmd + alt + o`)
- `ctrl + shift + a` - search action (`cmd + shift + a`)

### Tabs & Windows
- `ctrl + tab` - tab & tool switcher ⚡
- `alt + left/right` - go to previous/next tab (`ctrl + left/right`) ⚡
- `ctrl + alt + ]/[` - switch to previous/next IntelliJ IDEA window ⚡
- `f12` - go to previous tool window ⚡
- `escape` - go to editor (from tool window) ✔
- `shift + escape` - hide active (or last active) window ✔

### Single tab
- `ctrl + g` - go to line (`cmd + l`) ✔
- `alt + up/down` - go to previous/next method
- `ctrl + [/]` - move to code block start/end 
- `ctrl + shift + m` - move caret to matching brace
- `f2 / shift + f2` - next/previous highlighted error

### Recent locations
- `ctrl + alt + left/right` - navigate back/forward (`cmd + alt + left/right`) ✔
- `ctrl + shift + backspace` - navigate to last edit location (`cmd + shift + backspace`) ⚡
- `ctrl + e` - recent files popup (`cmd + e`) ⚡
    - `ctrl + e` - recent edited files
- `ctrl + shift + e` - recent locations popup (`cmd + shift + e`) ⚡
    - `ctrl + shift + e` recent edited locations

### Usage search
- `alt + f7` - find usages (tool window) ✔
- `ctrl + f7` - highlight usages in file (`cmd + f7`)
    - `f3` - next usage (`cmd + g`) ✔
    - `shift + f3` - previous usage (`cmd + shift + g`) ✔
- `ctrl + alt + f7` - show usages in file (popup) (`cmd + alt + f7`)

### Bookmarks
- `f11` - toggle bookmark (`f3`)
- `ctrl + f11` - toggle bookmark with mnemonic (`alt + f3`)
- `shift + f11` - show bookmarks (`cmd + f3`)
- `ctrl + 0-9` - go to bookmark


### Hierarchies
- `ctrl + f12` - file structure popup (`cmd + f12`) ✔
- `ctrl + h` - type hierarchy
- `ctrl + shift + h` - method hierarchy (`cmd + shift + h`)
- `ctrl + alt + h` - call hierarchy ✔



---

## General

- run anything (ctrl+ctrl)

- `alt + f1` - select current file or symbol in any view ⚡

- `ctrl + f4` - close active tab (`cmd + w`)

- `ctrl + alt + s` - open Preferences (`cmd + ,`)
- `ctrl + alt + shift + s` - open Project structure (`cmd + ;`)

- `alt + insert` - new file, source, diagram, ...  (`cmd + n)`
- `ctrl + alt + shift + insert` - new scratch file (`cmd + shift + n`)

- `alt + home` - jump to navigation bar

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
- refresh (cmd+r)

- ! switch between class and test class (shift+cmd+t)
