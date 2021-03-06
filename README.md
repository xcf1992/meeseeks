## Bash
add .inputrc, add  
"\e[A": history-search-backward  
"\e[B": history-search-forward  
to remember last command starts with prefix  

## Install Apps
1. Xcode  
2. WeChat
3. Sougou
4. Java - jre
5. Java - jdk
6. VS Code
7. iTerm
8. OneNote

## Config Mac
1. Settings > keyboard > shortcuts > input sources  
2. change cursor size: Accessbiliy > Display  

### Config zsh
#### set zsh as default  
Open /etc/passwd:  

sudo vi /etc/passwd  
Find the line with your username:  

username:x:1634231:100:Your Name:/home/username:/bin/bash  
and replace bash with zsh:  

username:x:1634231:100:Your Name:/home/username:/bin/zsh  
Log out and log in back for the changes to take effect.  
#### Install Oh-my-zsh  
Change .zshrc, ZSH_THEME="xcf"  
put xcf.zsh-theme under ~/.oh-my-zsh/themes  

### Config iTerm
1. Install brew
2. Install Git
3. Download iTerm color scheme: https://github.com/mbadolato/iTerm2-Color-Schemes
   go to preferences > Profiles > Colors > Color Presets > import > Argonaut
4. Preferences > Keys > Hotkey
5. set different color to cursor and cursor text
6. With iTerm2 3.1.4, setup the following without adding individual key mappings.  
   Go to Preferences > Profiles > Keys  
   Left/Right ⌥ Key: Select Esc+  
   With a new Terminal session you are now able to use:  
   Option ⌥ + f to Get Forward  
   Option ⌥ + b to Get Forward  
   Option ⌥ + Delete ⌫ to Delete Word  

### Config tmux
https://www.hamvocke.com/blog/a-quick-and-easy-guide-to-tmux/

1. resizing panes using mouse  
   One option for resizing panes is to use the mouse.   
   To do this, add these lines to your .tmux.conf:  
   set -g mode-mouse on  
   set -g mouse-resize-pane on  
   If you are on a Mac and the above doesn't work, use this instead (source):  
   set-option -g mouse on  
   Once this mode is on, simply click and drag on pane dividers to resize them.  
  
   set -g mouse on #for newer versions  
2. https://github.com/gpakosz/.tmux

### Config Vim
1. https://github.com/amix/vimrc  
2. add customize config my_configs.vim to ~/.vim_runtime/my_configs.vim  
3. change nerd tree file window position,  
   access the ~/.vim_runtime/vimrcs/plugins_config.vim file and change the NERDTree position in that file.
4. add ```let g:snipMate = { 'snippet_version' : 1 }``` to .vimrc

### Config Sublime
1. Remove right preview - Under the View menu there is an option to Show/Hide Minimap  
2. Use color scheme - Mariana  
3. Install Pretty Json Package  
   Install this packages via CMD + SHIFT + P > Install package > Search for Pretty JSON and install.  
   And then turn ugly json via CMD + CTRL + J  

### Config git
install meld from https://yousseb.github.io/meld/  
goto mac preference, change security and privacy to trust meld  
1. brew install git  
2. setup account and email  
   git config --global user.email "chenfu.xie@hulu.com"  
   git config --global user.name "chenfu.xie"  
3. setup ssh key  
   https://help.github.com/articles/error-permission-denied-publickey/  
4. Add git commands shortcuts: put .gitconfig under $HOME  

### Config VSCode
1. install bracket pair colorizer 2  
2. install one dark scheme  
3. install vscode-icons  
4. change settings of trailing spaces and auto save  

### Config Golang
https://rominirani.com/setup-go-development-environment-with-visual-studio-code-7ea5d643a51a
https://github.com/Microsoft/vscode-go

### Config python
python multiple version: https://realpython.com/intro-to-pyenv/
https://github.com/pyenv/pyenv/issues/849, pyenv init, and add the eval to the end of zsh file

install python virtualenvwrapper, https://virtualenvwrapper.readthedocs.io/en/latest/

install ipython, https://ipython.org/
