# GDB

https://darkdust.net/files/GDB%20Cheat%20Sheet.pdf

## Breakpoints
- `b/break main` - set break point at `main` function
- `b *main+20`  

## Running
- `r/run` - run the binary
- `r < FILE` - run the binary, read from file

## Stepping
- `s/step` - do one step (dive into functions)
    - `si` - step instruction
- `n/next` - do one step (skip functions)
    - `ni` - next instruction
- `finish` - continue until the current function returns
- `c/continue` - continue execution

## Examine memory
- x - examine
    - x/32 $esp
