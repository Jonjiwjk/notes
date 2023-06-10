![Vim Cheat Sheet](vim_cheat_sheet.pdf)

Vim is a Unix text editor that's included in Linux, BSD, and macOS. It's known for being fast and efficient, in part because it's a small application that can run in a terminal (although it also has a graphical interface), but mostly because it can be controlled entirely with the keyboard with no need for menus or a mouse.

# Normal Mode
The default mode that Vim starts in. It is accessible by pressing the "Esc" key. In this mode you can use commands to move around your document 

## Command list
## Syntax : [Command] [Count] [Motion] 
### Motions (File Movement)
 - **h** : moves back one character
 - **j** : moves down one line
 - **k** : moves up one line
 - **l** : moves forwards one character
 - **w** : moves forwards one word
 - **b** : moves backwards one word 

A motion can be executed with a number in front (es. 7k) to execute that command multiple times at once. For example, following our **Syntax**, i could input **d3j** and i would delete the line im currently on, plus the 3 below
### Commands (File Modification) 
File modification
 - **d** : deletes the selected text
 - **u** : undoes the last action
 - **r** : redoes the last action
 - **y** : "yanks" (copies) the highlighted text
 - **p** : pastes the text contained in the buffer. The buffer that the p command accesses is connected to both the yank and delete commands. This means that any text that gets deleted will replace any text that gets copied, since they share the same buffer
 - **a** : changes  to INSERT MODE, with the cursor 1 character to the right
 - **i** : changes to INSERT MODE
 - **v** : changes to VISUAL MODE
 - **Shift+v** : changes to VISUAL LINE MODE

# Insert Mode
In this mode, activated by pressing 'i' while in Normal Mode, you can modify your document. This is the only mode where commands dont work
# Visual Mode
In this mode, activated by pressing 'v' while in Normal Mode, you can select parts of your document.
# Visual Line Mode
In this mode, activated by pressing 'Shift+v' while in Normal Mode, you can select parts of your document.

# Command Mode
In this mode, activated by pressing ':' while in Normal Mode, you can execute different commands on your document 
