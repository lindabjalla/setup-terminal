Git is a version control system. We will be using it on the course. Version control systems help managing the development cycle.

You should have already downloaded and installed git when setting up your computer for the course.

Now we need to configure it.

## Step 1

The following two git commands should be run from the terminal. You should replace "Your Name Here" with your name and "your_email@example.com" with your email. 

`git config --global user.name "Your Name Here"`
Sets the default name for git to use when you commit

`git config --global user.email "your_email@example.com"`
Sets the default email for git to use when you commit

## Step 2

We are going to change our terminal from a bash terminal to zsh terminal. We can do this by opening System Preferences --> Users and Groups, unlock the pane by clicking on the padlock. Right click on your user in the list and choose advanced options and change from bin/bash to bin/zsh.

If you want you can also download and install a popular coding font none as [inconsolata](http://www.levien.com/type/myfonts/inconsolata.html) and setup terminal to use it via terminals preferences.

We are now going to extend zsh with oh-my-zsh.

Run the following command in terminal.

`curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh`

In terminal cd into the configuration directory for oh-my-zsh

`cd ~/.oh-my-zsh`

We will now copy and use a standard template

`cp templates/zshrc.zsh-template ~/.zshrc`

We will now create a new theme with some cool git features.

`subl themes/doubleended.zsh-theme`

The terminal command above will create a new empty theme called doubleended. We now need to copy in the contents of the file from [here](https://raw.githubusercontent.com/wgriffioen/dotfiles/master/doubleend.zsh-theme) and save.

`mkdir ~/bin`

`subl ~/bin/batcharge.py` 

The terminal commands above will create an empty file called batcharge.py. We now need to copy in the contents of the file from [here](https://raw.githubusercontent.com/tbranyen/dotfiles/master/.scripts/batcharge.py)

The last action is to edit our config file and tell it to use our theme.

`subl ~/.zshrc`

Edit the theme 

`ZSH_THEME="robbyrussell"` should be changed to `ZSH_THEME="doubleended"`