# VIM Learning
Written in VIM ... 

## VIM Arguments
vim -O file1 file2
- Open files in 2 windows at once


## VIM CMD LINE
windo difft 
- For every window do diff and highlight difference


## VIM ESC MODE


## Theory
- Basic syntaxt
`[count][operator][text object/motion]`


Examples:
- 6+ = 6x down to line start
- gUaW = capitalize a word
- 3ce = 3x change the word end
- 4$ = 4x go to the end of line
- d]m = delete to start of next mehtod
- % = jump to the next parent or bracket


### Operators
- c = change
- d = delete
- y = yank into register
- ~ = swap case
- gu = make lowercase
- gU = mkae uppercase
- ! = filter to external program
- < or > = shift left/right
- = = indent

### Text Objects
- a = word + space
- inner = only word

- aw = a word
- iw = inner word
- aW = a WORD
- iW = inner WORD
- ap or ip = a/inner paragraph
- ab or ib = a/inner bracket
- at or it = a/inner tag block

### Motions
- numbers are optional

- % = go to first matching pattern
- 3+ = down 3 to first non-blank char of line
- 3$ = to end of line
- 3f/F{char} = to next occuerence of {char}
- 3t/T{char} = to before next occurence of {char}
- 3h/j/k/l = left down up right
- ]m = go to beginning of next method
- w/W = go a word to the right
- b/B = go a word to the left
- e/E = go to the end of word

## GENERAL MOVEMENTS
- H,M,L = High,Middle,Low = Top,Center and Bottom of the screen
- h,j,k,l = up down left right
- CTRL+U/CTRL+D = half page scroll up/down
- CTRL+B/CTRL+F = full page scroll up/down

## SEARCHING
- :/<pattern> = search for pattern forward
- :?<pattern> = search forr pattern backward
- n,N = next, previous
- `*` = search forward for word under cursor
- \\# = search backward like *

## File editing
- :o[pen] = open file
- :fin[d] = find and open file
- CTRL+^ = switch between openned files


