# My Ubuntu Development Setup

## gedit
	* Display line numbers
	* Set tabwidth to 4
	* Set spaces instead of tabs
	* Enable auto indent
	* Disable backup copy
	* Set autosave to 10 minutes
	* Set editor font to 16
	* Set color scheme to Cobalt
	
	
## Vim	
### Install
    ```
    $ sudo apt-get install vim-gnome`
    ```
    
### Set preferences


## Git
### Install
    ```
    $ sudo apt-get install git-core`
    ```
    
### Set config
	
	
## Chrome
### Install

### Edit chrome settings
    * Set startup page
    * Enable always show bookmarks bar
    * Enable 'do not track' request
    * Disable offer to save pswd
    * Set font size to medium
    * Set page zoom to 125%
    
### Install extensions
 
 
## Solarized Theme   
### For terminal
    Source: [webup8](http://www.webupd8.org/2011/04/solarized-must-have-color-paletter-for.html)
    
    ```
    $ wget --no-check-certificate https://raw.github.com/seebi/dircolors-solarized/master/dircolors.ansi-dark
    $ mv dircolors.ansi-dark .dircolors
    $ eval `dircolors ~/.dircolors`
    ```
    
    ```
    $ git clone https://github.com/sigurdga/gnome-terminal-colors-solarized.git
    $ cd gnome-terminal-colors-solarized
    $ ./set_dark.sh
    ```
    
### For Vim
    Source: [vim-colors-solarized](https://github.com/altercation/vim-colors-solarized)
    
    ```
    $ git clone https://github.com/altercation/vim-colors-solarized
    $ cd vim-colors-solarized/colors
    $ mkdir ~/.vim/colors
    $ mv solarized.vim ~/.vim/colors/
    ```
    
    Edit ~/.vimrc
    ```
    syntax enable
    set background=dark
    colorscheme solarized
    ```

### For gedit
    Source: [solarized-gedit](https://github.com/mattcan/solarized-gedit)
    ```
    $ git clone git://github.com/mattcan/solarized-gedit.git
    $ mkdir -p ~/.local/share/gedit/styles
    $ cp solarized-* ~/.local/share/gedit/styles
    ```
    Set the Solarized colorscheme from Preferences
