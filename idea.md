# IntelliJ IDEA

https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf

## Editing

- `ctrl + space` - basic code completion
- `ctrl + shift + space` - smart code completion
    - `enter` - insert
    - `tab` - replace


- `ctrl + shift + enter` - complete statement (`cmd + shift + enter`)


- `alt + enter` - show intention actions and quick-fixes
- `ctrl + F1` - show descriptions of error or warning at caret (`cmd + F1`)
    - `alt + shift + enter` - apply suggested fix
  

- `ctrl + p` - parameter info (`cmd + p`)
- `ctrl + mouse` - brief info, resolves `var` type (`cmd + mouse`)
- `ctrl + q` - quick documentation lookup (`cmd + j`, `F1`)
- `alt + q` - context info (current method, class) (`ctrl + shift + q`)


- `alt + insert` - generate code (`cmd + n`)
- `ctrl + alt + t` - surround with (if, else, try, catch, ..) (`cmd + alt + t`)
- `ctrl + o` - override methods
- `ctrl + i` - implement methods


- `ctrl + /` - comment / uncomment with line comment (`cmd + /`)
- `ctrl + shift + /` - comment / uncomment with block comment (`cmd + alt + /`)


- `ctrl + w` - extend selection (`alt + up`)
- `ctrl + shift + w` - shrink selection (`alt + down`)


- `ctrl + alt + l` - reformat code (`cmd + alt + l`)
- `ctrl + alt + o` - optimize imports (`ctrl + alt + o`)
- `ctrl + alt + i` - auto-indent line(s) (`ctrl + alt + i`)


- `ctrl + c` - copy line (`cmd + c`)
- `ctrl + x` - cut line (`cmd + x`)
- `ctrl + shift + v` - paste from recent buffers ("local clipboard history") (`cmd + shift +v`)


- `ctrl + d` - duplicate line (`cmd + d`)
- `ctrl + y` - delete line (`cmd + backspace`)
- `ctrl + shift + j` - join lines
- `shift + enter` - start new line (the current line remains unchanged)
- `ctrl + enter` - new line, don't move the cursor (`cmd + enter`)


- `ctrl + shift + u` - toggle word (selected block) case


- `alt + mouse drag` - column (rectangular) select
- `alt + shift + insert` - column selection mode (`cmd + shift + 8`)


- `alt + shift + up/down` - swap lines
- `ctrl + shift + up/down` - swap methods/blocks (`cmd + shift + up/down`)


## Usage search

- search everywhere (shift+shift)
    - go to class (cmd+o)
    - go to file (shift+cmd+o)
    - go to symbol (alt+cmd+o)
    - find action (shift+cmd+a)
- find usages (tool window) - option+f7
- find usages (in file) - cmd+f7
- highlight usages in file (shift+cmd+F7)
    - cmd+g / shift+cmd+g - navigate forward/back

## Navigation

- go to editor  (from tool window) (esc)
- hide active or last active windows (shift+esc)
- go to declaration (ctrl+click, cmd+b)
- file structure popup (cmd+F12)
- call hierarchy: callers/callees (ctrl+option+h)
- ! switch between class and test class (shift+cmd+t)
- navigate back/forward (cmd+option+left / cmd+option+right)
- recent locations (shift+cmd+e)
- type hierarchy (ctrl+h)

F2/shift + F2

ctrl + tab


`cmd + shift + ]` - next tab
`cmd + shift + [` - previous tab

## General

- switch between tabs and tool windows (ctrl+tab)
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