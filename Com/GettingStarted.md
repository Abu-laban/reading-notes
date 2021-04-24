# Getting Started


## Download Git

In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.
- Git can be installed in three ways:

  - Install as a package
  - Install via another installer
  - Download and compile the source code.


## Mac OS X

* Terminal

  - The simplest method for installing Git on a Mac (for Mavericks 10.9 and above) is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.

* Git Website

   - You can also download Git by visiting this link and following the posted directions:
https://git-scm.com/download/mac

* GitHub

   - A third option is to install Git as part of the GitHub for Mac install. GitHub is repository hosting service, which we will discuss in a future section.
Download GitHub for Mac via the following link:
https://mac.github.com

## Windows

* Git Website

  - You can download Git by visiting this link and following the posted directions:
https://git-scm.com/download/win

* GitHub

  - Install Git as part of the GitHub for Windows install.
https://windows.github.com

## Linux

* Package Manager

  - You can try installing Git via your distribution’s inherent package management tool.

* For Fedora:

  - > $ sudo yum install git


* For Ubuntu:

  - > $ sudo apt-get install git

* Git Website

  - To download Git for Linux, visit this link and follow the posted directions:
https://git-scm.com/download/linux

## Graphical Clients
  - Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

* GUI Clients
  - You can access a variety of GUI clients for Mac, Windows, and Linux via the following link: https://git-scm.com/downloads/guis

##  Initial Customization
  - After making sure Git has been installed, you should perform some customization steps, which should only need to be completed once on any machine. To change settings, you can repeat these steps.

#### Configuration of Variables
An inherent Git tool called
   > git config 

allows the setting of configuration variables that control aspects of Git’s operation and look.

#### Identity Setting
After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

* Type the following into Terminal or Command Line:

> git config --global user.name "Jane Smith"
 git config --global user.email "example@email.com"


* To confirm that you have the correct settings, enter the following command:

> git config --global user.name (should return Jane Smith)
git config --global user.email (should return example@email.com)


By using the global option, these Git settings apply to anything on the system. To use different identity settings for a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.

## Default Text Editor
* Without configuration of a default text editor, Git will use the system’s default editor–most likely Vim. To configure a different text editor, such as Emacs, type the following into your Terminal or Command Line:

> <span>$</span> git config --global core.editor emacs

Note: For some editors, you may need to find specific instructions for default configuration.

## Check Settings
To check settings, use the 
> git config --list command.

Example:

> $ git config --list
user.name=Jane Smith
user.email=example@email.com
color.status=auto
color.branch=auto
color.interactive=auto
...

## Getting Help
There are three ways to get more information on a particular command, by accessing the manual:

> git help command
git command --help
man git-command