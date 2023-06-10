![Vim Cheat Sheet](vim_cheat_sheet.pdf)

Vim is a Unix text editor that's included in Linux, BSD, and macOS. It's known for being fast and efficient, in part because it's a small application that can run in a terminal (although it also has a graphical interface), but mostly because it can be controlled entirely with the keyboard with no need for menus or a mouse.

# Normal Mode
The default mode that Vim starts in. It is accessible by pressing the "Esc" key. In this mode you can use commands to move around your document 

## Command list
#### Syntax : [Command] [Count] [Motion] 
Motions (File Movement)
 - h : moves back one character
 - j : moves down one line
 - k : moves up one line
 - l : moves forwards one character
 - w : moves forwards one word
 - b : moves backwards one word 

A motion can be executed with a number in front (es. 7k) to execute that command multiple times at once. For exapmle, following our **Syntax**, i could input **d3j** and i would delete the line im currently on, plus the 3 below
File modification
 - d
 - u
 - r

# Insert Mode
In this mode, activated by pressing 'i' while in Normal Mode, you can modify your document
# Visual Mode
In this mode, activated by pressing 'v' while in Normal Mode, you can select parts of your document.
# Command Mode
In this mode, activated by pressing ':' while in Normal Mode, you can execute different commands on your document 
