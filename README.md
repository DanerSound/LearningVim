# LearningVim

****I want to learn vim or I will die trying****

###### *I raccomend to use vimtutor as the best guide for vim*

## Install vim

**Debian**: `sudo apt install vim`

## Open a file

On a terminal write:
```
vim <path_to_file>
```
This will open the file you want to edit with vim.

## Navigations

Rule #1: *Never use arrow keys.*

From now on i disable the up, down, left, right arrow and I will use only the h, j, k, l.

```
To move the cursor, press the h,j,k,l keys as indicated. 
             ^
             k              Hint:  The h key is at the left and moves left.
       < h       l >               The l key is at the right and moves right.
             j                     The j key looks like a down arrow.
             v
```
(Quote: [Vimtutor](#references))

If hold a move keys it repets the move.

## Exiting Vim

***Tip: When you are in Normal Mode you can execute vim commands. Press the <ESC> key to make sure you are in Normal Mode***

Normal Mode:
* Exit without save (trash all changes): `:q!`
* Exit with save (save the changes): `:wq`

## Text Editing

Normal Mode:
* Delete single focus character: `x`
* Enter in Insert Mode: `i`
* Append some text next to the character focused 

#### References
* Vimtutor: you can easy run vimtutor from your terminal and get all the documentations and help of the vim editor
* Video of [DistroTube](https://www.youtube.com/channel/UCVls1GmFKf6WlTraIb_IaJg): [The Vim Tutorial - Part One - Basic Commands](https://www.youtube.com/watch?v=ER5JYFKkYDg)

