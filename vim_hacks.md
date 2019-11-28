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
- ci'' = (second quote is just escape) change inside quote the text


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
- CTRL-E/CTRY+Y = scrol without moving cursor

## SEARCHING
- :/<pattern> = search for pattern forward
- :?<pattern> = search for pattern backward
- n,N = next, previous
- `*` = search forward for word under cursor
- \\# = search backward like *

## Bookmarks - like in books where I left my reading?
- m<char> = define postion
- `<char> = return to position
- :marks = show current tags

## File editing
- :o[pen] = open file
- :fin[d] = find and open file
- CTRL+^ = switch between openned files

## TAGS
- Good for beginners
- Navigate in projects with CTRL-] and CTRL-t

## Changes
- :jumps - see all the movements in VIM
- :changes - see all the changes
- g; and g, - cycle through changes
- CTRL-I, CTRL-O = jump forward/backward, usefull if you go to another file and wanna come back


## VIM Buffers
- Buffers are regular browser Tabs
- Windows are buffer viewports
- Buffers are historic view of every edited file 

- :buffers - print buffers
- :bn - go to next buffer
- :b <filename>  - go to buffer filename
- :bd - delete current buffer


- Arguments represents openned files
- Stable buffer list
- :arga <filename> - add filename to arg list
- :n  - go to next file in arg list

- Windows is just splitting buffers
- CTRL+W s - split windows horizontally
- CTRL+W v - split windows vertically
- CTRL+W q - close window
- CTRL+W r - rotate windows = exchange windows positions
- CTRL+W w - move cursror between windows
- :windo <cmd> - execute command for all windows
- :sf <file> - split window and find file


- TABs are window containers
- Tabs are couple of windows, like 1 TAB is 1 IDE
- gt - go to next tab
- gT - go to prev tab
- :tabc - close tab
- :tabe - open tap
- :tabo - close all other tabs
