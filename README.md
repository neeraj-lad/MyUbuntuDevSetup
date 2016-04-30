# My Ubuntu Development Setup

## gedit
--------
	* Display line numbers
	* Set tabwidth to 4
	* Set spaces instead of tabs
	* Enable auto indent
	* Disable backup copy
	* Set autosave to 10 minutes
	* Set editor font to 16
	* Set color scheme to Cobalt
	
	
## Vim
------
### Install
    $ sudo apt-get install vim-gnome
    
### Setup .vimrc


## Git
------
### Install
    $ sudo apt-get install git-core
    
### Set config
    $ git config --global user.name '<user name>'
    $ git config --global user.email '<user email>'	

### Enable Credential Helper
    $ git config --global credential.helper cache
    $ git config --global credential.helper 'cache --timeout=3600'

	
## Chrome
---------
### Install

### Edit chrome settings
    * Set startup page
    * Enable always show bookmarks bar
    * Enable 'do not track' request
    * Disable offer to save pswd
    * Set font size to medium
    * Set page zoom to 150%
    
### Install extensions
 
 
## Solarized Theme
------------------
### For terminal
Source: [webup8](http://www.webupd8.org/2011/04/solarized-must-have-color-paletter-for.html)
    
    $ wget --no-check-certificate https://raw.github.com/seebi/dircolors-solarized/master/dircolors.ansi-dark
    $ mv dircolors.ansi-dark .dircolors
    $ eval `dircolors ~/.dircolors`
   
 
    $ git clone https://github.com/sigurdga/gnome-terminal-colors-solarized.git
    $ cd gnome-terminal-colors-solarized
    $ ./set_dark.sh
    
### For Vim
Source: [vim-colors-solarized](https://github.com/altercation/vim-colors-solarized)
    
    $ git clone https://github.com/altercation/vim-colors-solarized
    $ cd vim-colors-solarized/colors
    $ mkdir ~/.vim/colors
    $ mv solarized.vim ~/.vim/colors/
   
 
    Edit ~/.vimrc
    syntax enable
    set background=dark
    colorscheme solarized

### For gedit
Source: [solarized-gedit](https://github.com/mattcan/solarized-gedit)

    $ git clone git://github.com/mattcan/solarized-gedit.git
    $ mkdir -p ~/.local/share/gedit/styles
    $ cp solarized-* ~/.local/share/gedit/styles


    Set the Solarized colorscheme from Preferences
 
# Compilers
----------- 
    

# Ubuntu
--------
## Ubuntu Settings
    * Set Time & Date settings
    * Set Lock screen time
    * Disable Dash online search
    * Setup Déjà Dup
    
## Install the Inconsolata font
    sudo apt-get install fonts-inconsolata
    sudo fc-cache -fv 
    
    Set terminal to use it. Set Inconsolata Medium with font size of 19
     
## Caffeine Indicator
Source: [ubuntuhandbook](http://ubuntuhandbook.org/index.php/2015/01/install-caffeine-indicator-ubuntu-14-04/)
    
    $ sudo add-apt-repository ppa:caffeine-developers/ppa
    
    $ sudo apt-get update
    $ sudo apt-get install caffeine
    
    Add Caffeine to the Startup Applications.
    
## Ubuntu Indicator Applets
    * Multiload
    $ sudo apt-get install indicator-multiload
    
## Stopwatch


# Python
--------
## Install pip
    sudo apt-get install python-pip
    
## Install virtualenv
    sudo pip install virtualenv
    
    mkdir ~/.virtualenvs

## Install virtualenvwrapper
    sudo pip install virtualenvwrapper
    
    #Set WORKON_HOME to your virtualenv dir
    export WORKON_HOME=~/.virtualenvs
    
    #Add virtualenvwrapper.sh to .bashrc
    . /usr/local/bin/virtualenvwrapper.sh
    

# Topcoder
----------
## Install Java Webstart

## Setup Vimcoder


# LAMP Stack
------------
Source: [howtoubuntu.org](http://howtoubuntu.org/how-to-install-lamp-on-ubuntu)

## Install Apache
    sudo apt-get install apache2
    
## Install MySQL
    sudo apt-get install mysql-server

## Install PHP
    sudo apt-get install php5 libapache2-mod-php5
    
## Restart Apache
    sudo /etc/init.d/apache2 restart
    
## Check
    Check Apache is working:
    Navigate to http://localhost/
    
    Check PHP is working:
    php -r 'echo "\n\nYour PHP installation is working fine.\n\n\n";'
    
# Adobe Brackets
----------------
Source: [webupd8](http://www.webupd8.org/2013/11/install-brackets-in-ubuntu-via-ppa-open.html)

    sudo add-apt-repository ppa:webupd8team/brackets
    sudo apt-get update
    sudo apt-get install brackets
