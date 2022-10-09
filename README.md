# Terminal and Shell Commands Cheatsheet For Mac Users

The shell takes commands and executes them against the operating system. The termianl is a program that wraps the shell. This list inclides common commands and scripts for learning more about navigating the terminal.

> A resource for Terminal and Shell command scripting. 

[Free resource to study shell commands and more!](https://learnshell.org)

- Clear the window: **( control + l )** 
- Also clears the window: `clear` 
- Open a new window virtically: **( cmd + t )**
- Open another virticle window: **( cmd + d )**
- Open a horizontal window: **( shift + cmd + d )**
- Delete a window: **( cmd + w )**
- How to delete one word at a time going forwards: **( option + d )**
- How to delete one word at a time going backwards: **( option + backspace )**
- Naviagte to the beggining of a line in terminal: **( control + a )**
- Naviagte to the end of a line in terminal: **( control + e )**
- How to scroll up and down in the window: **( shift + arrow buttons )**
- How to get out of vi: **( cmd + :q! )**
- How to move cursor forwards or backwards over text to delete or just move back: **( command + b )**

--------------------------------------------------------------------------------------------------------
## iTerm
- iTerm reccomended as a better terminal
<br>
[download iTerm]("https://iterm2.com/downloads.html")
- How to check if you're using bash or zsh: in the iTerm window 

`echo $SHELL`

- ** zsh ** everything applicable to zsh is applicable to bash.
- How to change from bash to zsh: in the iTerm window

`chsh -s /bin/zsh`

--------------------------------------------------------------------------------------------------------
## On My ZSH
#### an open soource framework for mamanging your zsh configuration
- How to install **Oh My ZSH**
<br>
` sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" `

- Get the docs for Oh My ZSH:
`vi .zshrc` 
<br>
- [customizing your Oh MY zsh theme](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)

--------------------------------------------------------------------------------------------
## Introduction To Shell Commands
1. How to access the manual page... `man`
2. "What manual page do you want?" `man` + **( command )** type man and the command you want the manual for
3. type `q` to exit/quit
- start typing a file name then press **( tab )** to finish the file name
- `date` gives the current date and time
- `cal` shows your calander add the year ex: `cal 2022` for full years calander
- `whoami` gives the user name

## Working with directories
- `.` your current directory
- `pwd` gets working path directory
- `ls` shows the contents inside of the current working directory
- `ls -a` shows files that begin with a "."
- `ls -al` shows more details about the files
- `cd` change directory/file/folder
- `cd ~ ` go back to the root directory
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
- `cat` **( + file_name )** shows the contents of your file
