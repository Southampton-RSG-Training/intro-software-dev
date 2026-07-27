---
title: Setup
---


## Software Setup

### Bash Shell 

For this workshop, you will need to be able to interact with your computer through a terminal using the Bash Shell. See below for instructions to install and/or open a terminal on your operating system:

:::::::::::::::: spoiler

### Windows

We’ll be using Git Bash to access a terminal on Windows machines. Go to [git for windows](https://gitforwindows.org/) and click Download, then install it. Most of the options can be left on default, but be sure you check these:

- Choosing the default editor used by Git: Make sure Nano is selected from the drop-down. If you’re comfortable with other editors, feel free to change it, but we recommend Nano - we use it as it’s present on Windows, Mac and Linux. If you change it, you might not quite match what we’re doing on-screen.
- Adjusting your PATH environment: Make sure Git from the command line and also from 3rd-party software is selected.
- Choosing HTTPS transport backend: Make sure Use the native Windows Secure Channel Library is selected.
- Configuring the terminal emulator to use with Git Bash: Make sure Use Windows’ default console window is selected.


::::::::::::::::::::::::

:::::::::::::::: spoiler

### MacOS

Open the “Terminal” application, which can be found in the “Utilities” folder which is in your “Applications” folder.

::::::::::::::::::::::::


:::::::::::::::: spoiler

### Linux

This will depend on the Linux distribution you are running, but you should be able to find a “Terminal” application in your desktop’s application menu.

::::::::::::::::::::::::

### Git

First make sure you can open a terminal and access the Bash Shell (instructions above). Then follow the instructions for your operating system below:

:::::::::::::::: spoiler

### Windows

We’ll be using Git Bash for both git and a shell to run it in. If you’ve already installed Git Bash then go to the next section. 

::::::::::::::::::::::::

:::::::::::::::: spoiler

### MacOS

To use Git you must install the Apple Command Line Tools, this may take a few minutes.

You can obtain these [from Apple](https://developer.apple.com/download/more/?name=command%20line%20tools%20for%20xcode%2012) (requires your Apple ID)

- Select Command Line Tools for Xcode 12 (or higher) and click the link to download the dmg archive.
- If prompted, choose to allow downloads from developer.apple.com
- Open the downloaded dmg archive from the Downloads folder
- Double-click the Command Line Tools.pkg icon to install

Alternatively, you can install the tools from the command line:

```bash
xcode-select --install
```

::::::::::::::::::::::::


:::::::::::::::: spoiler

### Linux

Git comes pre-installed on most Linux distributions. You can test if it’s installed by running `git --version`. If it’s not installed, you can install it by running `sudo apt-get install git` or `sudo yum install git`, depending on your distribution.

::::::::::::::::::::::::

### GitHub

We’ll be using the website [GitHub](https://github.com/) to host, back up, and distribute our code. You’ll need to create an account there. As your GitHub username will appear in the URLs of your projects there, it’s best to use a short, clear version of your name if you can.

### Python

The "Anaconda3" package provides everything Python-related you will need for the workshop. To install Anaconda, follow the instructions below.

:::::::::::::::: spoiler

### Windows

- Head to the [Anaconda Download Page](https://www.anaconda.com/products/individual) and download the latest Anaconda Windows installer. 
- Double-click the installer and follow the instructions. 
- **When asked “Add Anaconda to my PATH environment variable”, answer “yes”. It will warn you not to, but it's required for it to be found by git bash** 
- Once the Anaconda installation is finished you will be asked if you want the installer to initialize Anaconda3 by running conda init? You should select yes. 

Alternatively/additionally you will need to run the following command in Git Bash

```bash
conda init bash
```

- Close and reopen any open terminals to reload the updated PATH and allow the installed Python to be found.

To test whether the python installation was successful, open Git Bash and run the following command:

```bash
cd ~
python
```

In some cases, Git Bash will hang on this command and not launch the Python interpreter. In this case close and reopen Git Bash and issue the following commands:

```bash
cd ~
echo 'alias python="winpty python.exe"' >> ~/.bash_profile
source .bash_profile
python
```

For older versions of git bash you will need to use .bashrc rather than .bash_profile

You can type the following to exit the python interpreter:

```
quit()
```


::::::::::::::::::::::::

:::::::::::::::: spoiler

### MacOS

#### Mac OS Intel
Download the latest Anaconda Mac OS X installer. Double-click the .pkg file and follow the instructions.

#### Mac OS M1
If you have a M1 Mac you need a specific version of Anaconda follow the link below. 

[M1 Compatible Anaconda](https://repo.anaconda.com/archive/Anaconda3-2022.05-MacOSX-arm64.pkg)

Once the Anaconda installation is finished you will be asked if you want the installer to initialize Anaconda3 by
running conda init? You should select yes.


::::::::::::::::::::::::


:::::::::::::::: spoiler

### Linux

Download the latest Anaconda Linux Installer.

Install via the terminal like this (you will need to change the version number to the latest version):

First move to the folder where you downloaded the installer, this is likely to be the Downloads folder e.g.

```bash
cd ~/Downloads
```

```bash
bash Anaconda3-2021.11-Linux-x86_64.sh
```

Answer ‘yes’ to allow the installer to initialize Anaconda3 in your .bashrc.

::::::::::::::::::::::::

## Data Sets

### Download Data for Bash Shell Lesson

Open a terminal and type the following into the prompt that appears (pressing enter/return after each line):

```bash
cd
git clone https://github.com/Southampton-RSG-Training/shell-novice.git
```

`cd` will move to your home directory, and `git clone` will download a copy of the materials.

This should download all the content for the lesson to a new directory. 

### Download Data for the Python Lesson

To download the data for the Python lesson, open a terminal on your machine, and enter:

```bash
cd
git clone https://github.com/Southampton-RSG-Training/python-novice
```



