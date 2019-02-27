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

There are several ways to repeats a motion: hold the motion key or type a number before a motion.
```
<motion>
```
or
```
<number><motion>
```

For example: You want to move the cursor to the start of the third word ahead, you can type `3w`. In the same way you can move to the 10th line after the line where you are by type `10j`. 


## Exiting Vim

###### **On Normal Mode**
--------------------------------------------------
#### Exit without save (trash all changes): 
```
:q!
```
--------------------------------------------------
#### Exit with save (save the changes): 
```
:wq
```
--------------------------------------------------


## Text Editing and Commands

###### **On Normal Mode**
--------------------------------------------------
#### Delete single focus character: 
```
x
```
--------------------------------------------------
#### Delete operator (to know more go to [Operators](#operators) paragraph):
```
d<motion>
```
--------------------------------------------------
#### Enter in **Insert Mode** (insert before the cursor): 
```
i
```
--------------------------------------------------
#### Enter in **Insert Mode** next to the character focused (append after the character):
```
a
```
--------------------------------------------------
#### Append text to the line focused (this will put you on **Insert Mode** at the end of the line of the character focused):
```
A or Shift+a
``` 
--------------------------------------------------
#### Undo last commands executed:
```
u
```
--------------------------------------------------
#### Undo a whole line and return the line to its original state:
```
U or Shift+u
```
--------------------------------------------------
#### Redo last commands, that is undo the undo's:
```
CTRL+r
```
You can keep CTRL key and hitting *r* a number of time to redo multiple times.

--------------------------------------------------
#### Put the previously deleted text after the cursor:
```
p
```
--------------------------------------------------
#### Replace command allows to insert a new character above the character focused:
```
r<new_character>
```
--------------------------------------------------
#### Show the position in the file and status of the file:
```
Ctrl+g
```
--------------------------------------------------
#### Move to the bottom of the file:
```
G or Shift+g
```
--------------------------------------------------
#### Move to the start of the file:
```
gg
```
--------------------------------------------------
#### Move to a defined line:
```
<number>G or <number>+Shift+g
```
--------------------------------------------------
#### Search command:

*Forward direction*
```
/<string_to_search>
```
*Backward direction*
```
?<string_to_search>
```
To search for the same phrase again:
```
n
```
To search for the same phrase in the opposite direction:
```
N or Shift+n
```
--------------------------------------------------
#### Return to the previous position:

*Forward direction*:
```
Ctrl+o
```
and *Backward direction*:
```
Ctrl+i
```
--------------------------------------------------
#### Mach parentheses search command:
```
%
```
This command will place the cursor on any *(*, *[*, *{* in the line below marked.

--------------------------------------------------

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

--------------------------------------------------

###### **On Normal Mode**

#### Delete operator: 

```
d<motion>
```
or
```
d[number]<motion>
```

There are several **motion** for the delete operator:
- `w` - delete until the start of the next word, excluding its first character.
- `e` - delete to the end of the current word, including the last character.
- `$` - delete to the end of the line, including the last character.
- `0` - delete from the start of the line to the character where the cursor is.
- To know all the motions go to [Navigations and motions](#navigations-and-motions)

To delete the entire line you can use the command:
```
dd
```
Or delete more the 1 line:
```
<number>dd
```

--------------------------------------------------

#### Change operator:
```
c<motion>
```
or
```
c[number]<motion>
```

This operator delete the selection made with the motion and put you in the **Insert Mode**. It is something like delete and replace command.

It can be use all the motion, some example they can be:
- `w` - replace until the start of the next word, excluding its first character.
- `e` - replace to the end of the current word, including the last character.
- `$` - replace to the end of the line, including the last character.
- `0` - replace from the start of the line to the character where the cursor is.
- To know all the motions go to [Navigations and motions](#navigations-and-motions)

--------------------------------------------------

## References
* **Vimtutor**: you can easy run vimtutor from your terminal and get all the documentations and help of the vim editor
* **Video of [DistroTube](https://www.youtube.com/channel/UCVls1GmFKf6WlTraIb_IaJg)**: [The Vim Tutorial - Part One - Basic Commands](https://www.youtube.com/watch?v=ER5JYFKkYDg)

