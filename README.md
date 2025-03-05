This suite offers the ability to track and traverse a history of the directories you've been to,
by overloading the cd command.  Additionally, it offers the ability to mark directories
with a single letter, both ephemerally, and persistently, through lower and upper case
single letter marks respectively.

# Installation
Simply source the script from your bashrc.
```bash
git clone https://github.com/superboot/extended-cd ~/.extended-cd
echo 'source ~/.extended-cd/extended-cd' >> ~/.bashrc
```

# Usage

## COMMANDS:
- m [a-zA-Z]               --  Mark the current directory
- m /path/to/dir [a-zA-Z]  --  Mark the supplied path with the supplied single letter.
- delm [a-zA-Z]            --  Remove the mark from the system.
- cd [a-zA-Z]              --  Change directory to the directory saved in the mark.
- cd [1..999]              --  Change directory to the directory at position N in the history stack. Appends to the end of the stack.
- cd ,                     --  Change directory to the most recently modified directory in the PWD.
- cd ,-                    --  Recursively change directory to the most recently modified directory in the PWD.
- ,                        --  Change directory to the most recently modified directory in the PWD.
- ,,                       --  Recursively change directory to the most recently modified directory in the PWD.

## KEY BINDINGS:
- alt-p    --  Print position in directory stack (max size 9 lines).
- alt-P    --  Print position in directory stack. (max size, a full screen).
- alt-o    --  Navigate backward one step in the history.
- alt-i    --  Navigate forward one step in the history. 

