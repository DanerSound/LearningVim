# LearningVim

[![Vim](https://www.vim.org/images/vim_header.gif)](https://www.vim.org/)

****I want to learn vim or I will die trying****

###### *I raccomend to use vimtutor as the best guide for vim*
###### *Whatever happens, remember to press `<ESC>` to return on Normal Mode*

## Install vim

**Debian**: `sudo apt install vim`

## Open a file

On a terminal write:
```
vim <path_to_file>
```
This will open the file you want to edit with vim.

## Navigations and Motions

***Tip1: Never use arrow keys.***

***Tip2: When you are in Normal Mode you can execute vim commands. Press the `<ESC>` key to make sure you are in Normal Mode***

All the moves are intended to be use in **Normal Mode**.

```
To move the cursor, press the h,j,k,l keys as indicated. 
             ^
             k              Hint:  The h key is at the left and moves left.
       < h       l >               The l key is at the right and moves right.
             j                     The j key looks like a down arrow.
             v
```
(Quote: [Vimtutor](#references))

The move from a character to another is called **motion**.

All the motions that you can use are:
* `h/j/k/l` - in order move left/down/up/right
* `w` - move to the start of the next word 
* `e` - move to the end of the next word
* `$` - move to the end of the line
* `0` - move to the start of the line

If hold a motions keys it repeats the move.

## Exiting Vim

**Normal Mode:**
* Exit without save (trash all changes): 
```
:q!
```
* Exit with save (save the changes): 
```
:wq
```

## Text Editing

**Normal Mode:**
* Delete single focus character: 
```
x
```
* Delete operator ([Operators](#operators)):
```
d<motion>
```
* Enter in **Insert Mode** (insert before the cursor): 
```
i
```
* Enter in **Insert Mode** next to the character focused (append after the character):
```
a
```
* Append text to the line focused (this will put you on **Insert Mode** at the end of the line of the character focused):
```
A or Shift+a
``` 

## Operators

```
Many commands that change text are made from an operator and a motion.
```
(Quote: [Vimtutor](#references))

###### All the motions are in the [Navigation and motions](#navigation_and_motions) section.

**Format:**
```
<operator><motion>
```

**Normal Mode:**
* Delete operator: 
	```
	d<motion>
	```

	There are several **motion** for the delete operator:
	- `w` - delete until the start of the next word, excluding its first character.
	- `e` - delete to the end of the current word, including the last character.
	- `$` - delete to the end of the line, including the last character.

-------------------------------------------------------------------

#### References
* **Vimtutor**: you can easy run vimtutor from your terminal and get all the documentations and help of the vim editor
* **Video of [DistroTube](https://www.youtube.com/channel/UCVls1GmFKf6WlTraIb_IaJg)**: [The Vim Tutorial - Part One - Basic Commands](https://www.youtube.com/watch?v=ER5JYFKkYDg)

