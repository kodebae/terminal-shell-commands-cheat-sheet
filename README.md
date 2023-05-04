# 🧑‍💻 Terminal and Shell Commands Cheatsheet **For Mac Users** 

The shell takes commands and executes them against the operating system. The terminal is a program that wraps the shell. This list includes common commands and scripts for learning more about navigating the terminal.

> This Repo is a resource for Terminal and Shell command scripting. To make a contribution to this directory, please make a pull request. Requests will be reviewed in the order received.

## Resource List
-------------------------------------------------------------------------------------------------------
[Learn Shell.Org](https://learnshell.org)


## Basic Commands
- Clear the window: **( control + l )**
- Also clears the window: `clear` 
- Open a new window vertical: **( cmd + t )**
- Open another vertical window: **( cmd + d )**
- Open a horizontal window: **( shift + cmd + d )**
- Delete a window: **( cmd + w )**
- How to delete one word at a time going forwards: **( option + d )**
- How to delete one word at a time going backwards: **( option + backspace )**
- Navigate to the beginning of a line in terminal: **( control + a )**
- Navigate to the end of a line in terminal: **( control + e )**
- How to scroll up and down in the window: **( shift + arrow buttons )**
- How to get out of vi: **( cmd + :q! )**
- How to move cursor forwards or backwards over text to delete or just move back: **( command + b )**

--------------------------------------------------------------------------------------------------------
## Using & Installing iTerm
- iTerm recommended by developers as a better terminal
<br>
[download iTerm]("https://iterm2.com/downloads.html")
- How to check if you're using bash or zsh: in the iTerm window 

`echo $SHELL`

- ** zsh ** everything applicable to zsh is applicable to bash.
- How to change from bash to zsh: in the iTerm window

`chsh -s /bin/zsh`

--------------------------------------------------------------------------------------------------------
## Using & Installing On My ZSH
#### An open source framework for mananging your zsh configuration
- How to install **Oh My ZSH**
<br>
` sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" `

- Get the docs for Oh My ZSH:
`vi .zshrc`
<br>
- [customizing your Oh MY zsh theme](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)

--------------------------------------------------------------------------------------------
## Introduction To Shell Commands
1. How to access the manual page... this will work for any command to learn more info about how each command works `man`
2. "What manual page do you want?" `man` + **( command )** type man and the command you want the manual for
3. type `q` to exit/quit
- start typing a file name then press **( tab )** to finish the file name
- `date` gives the current date and time
- `cal` shows your calender add the year ex: `cal 2022` for full years calender
- `whoami` gives the user name
- `history` gives the history of all terminal commands ran and a number for each one
- `!155` to run that command again
- `history | grep "grep"` shows the history of the grep command
- `!!` gives you the previous command ran in the terminal
- `^rep^grep` replaces *rep* with *grep* in the last command ran

## Working with directories (*folders and directories used interchangablity*)
- `.` your current directory
- `pwd` gets working path directory
- `ls` shows the contents inside of the current working directory
- `ls -a` shows files that begin with a "."
- `ls -al` shows more details about the files
- `cd` change directory/file/folder
- `cd ~` go back to the root directory
- `cd ..` go back one level in the directory
- `cd ../..` go back two levels, keep chaining on /.. for more levels
- `cd -` go back to the previous folder
- `mkdir` **( + file_name )** makes a new file in whatever directory you are currently in
- `mkdir -p` **( + file_name/another_file/one_more_file )** creates sub directories
- `rm + -rf` **( + file_name )** removes a file and it's root directory **CAN NOT BE UNDONE**
- `mv` **( + file_1 + file_2 )** moves file_1 inside of file_2
- `tree -- help` to see tree commands, will need to install tree with Homebrew
- `mv` **( rename_this + new_file_name )** How to give your file a new name

## Working with files 
- `touch` **( my_file.py )** creates a new my_file.py file
- `rm` ( file_name* ) removes any file that starts with "file_name"
- `echo` prints the specified text string before listing of all the files in the current working directory
- **( > )** override
- **( >> )** append
- `cat` **( + file_name )** view the contents of your file
- `less` **( + file_name )** view less of the content, press spacebar to paginate over the file contents
- `head` **( + file_name )** view the first 10 lines of the file contents
- `tail` **( + file_name )** view the last 10 lines of the contents
- `cp` **( + file_to_copy + new_file_name )** copies the contents of one file to a new file
- `cp` **( * .file_extension + folder_name )** moves all files with this file extension to the specified folder. 
- `cp -r` **( * folder_name + new_folder )** moves all folders to a new folder
- `find .` lists every file in the current working folders
- `find . -type f -name file_name.ext` finds the specified file/s *sub -iname in place of -name to ignore the case sensitivity if files* *add -delete* to remove the file instead
- `find . -type f -name "*.ext"` finds all files with the specified extension
- `find . -type f -empty` finds all of the empty files *remove -type to find all empty folders*

### RegEx
- `man grep` to get the manual for this command *grep stands for, global regular expression print* works with both folders and files
- `grep -r` **( + "REGEX Goes here" + file_name )** and is used to search recursive text within files
- `grep -ni` **( + "REGEX" )** search for the line number and ignore the letter case
- `grep -rni -A 1 -B 1` **( + "REGEX" )** search for one line before and one line after the results adjust the numbers as needed
- `grep` works with REGEX and any other text as well


