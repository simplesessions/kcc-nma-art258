#### KCC NMA ART-258
# Week 04: Class: 02

## The Command Line Interface (CLI)

The CLI is a text-based prompt that lets you control your computer in various ways. The CLI is the text-based equivalent/companion to the GUI, or Graphical User Interface, which consts of windows, buttons, and everything else that you usually control with your mouse.

During this class, it's important to get used to certain conventions that let you do two fundamental functions:

- Traversing your comptuer (finding your folders and files)
- Issue commands to the CLI

Over the rest of the course, we'll be using the CLI to run various commands to __compile__ our source files (We'll go over this concept later).

### Traversing Your Computer

Fortunately, getting around in both Mac and Windows is very similar. I'll list some terms here for reference, and we'll go over how these are used in class.

#### Before Getting Started

__[Download Node.js](https://nodejs.org/en/)__

Since we'll be using Node.js in this class, which is a program that will be highly-utilized through the CLI in this class, be sure to download and install this first before getting started.

#### Opening the CLI

- Windows
	- Since we're using Node in this class, hit the Windows button (Start button), and open the __Node.js command prompt__. Be sure not to open anything else named "Node.js"
- Mac
	- __If this is your first time opening the CLI, do the following step. Otherwise, just open Terminal in your Applications/Utilities folder__.
		- Open Terminal, found in your Applications folder, and paste the following code, then hit Return.
		- Close Terminal, then open it again.

  - ```
    touch ~/.npmrc
    echo "prefix = ~/.npm-global" >> ~/.npmrc
    mkdir -p ~/.npm-global/bin
    touch .profile
    echo "export PATH=$PATH:$HOME/.npm-global/bin" >> ~/.profile
    source ~/.profile
    

#### Commands

- General Concepts
	- `.` - current directory
	- `..` - previous directory
- General Commands
	- `cd [<path>]` - change directory. Running this on the mac
	- `mkdir <path>` - make directory
- Mac-specific Commands
	- `ls [<path>]` - list everything in your directory
                - `ls -la [<path>]` - list everything in the path. including hidden files, and in a vertical list format
	- `open <path>` - open the location specified by `<path>` in Mac
	- `cd` - change to yoru home directory
- Windows-specific Commands
	- `dir` - list everything in your directory
	- `rmdir <path>` - remove directory
	- `cd /d %USERPROFILE%` - change to your home directory
	- `explorer <path>` - open the location specified by `<path>` in Windows

#### Notes

- In Windows, directory separators use backslashes – `\`
- On the Mac, directory separators use (forward) slashes –  `/`

#### See More

- [Windows CLI Tutorial](https://www.youtube.com/watch?v=MBBWVgE0ewk)
- [macOS CLI Tutorial (Terminal)](https://www.youtube.com/watch?v=jDINUSK7rXE)


#### Homework

Try these different exercises within the CLI to get used to the CLI environment:

- How do you get to your home folder (aka your user's folder)?
- Make a folder on the desktop without first going to the desktop
- `cd` to your newly created folder while starting from your home folder
- From your newly created folder, what are two ways you could traverse back to your home folder with one command?
- Open your newly created folder in the GUI from the CLI.

The best way to get used to using the CLI is with practices, so try these exercises a few times over and over until you get used to using all the commands necessary to accomplish these tasks. Good luck!

## npm – Node Package Manager

NPM - Node Package Manager - is a program, installed when you install [Node.js](http://nodejs.org), that allows you to install various programs and plugins you'll be using to accomplish various web-development tasks.

You'll often see these programs and plugins refered by the following names: packages, modules, and node modules. For our purposes, these are all synonymous.

### Syntax

`__npm install__`

Running `npm install` by itself will attempt to find a file within the directory in which its run called `package.json`, which usually has a list of _dependencies_ that npm will start to install. _dependencies_ are pieces of software that your website depends on to function as intended. Because `package.json` keeps track of this list of _dependencies_, you'll have an easier time referencing all the software needed for your site to run. More importantly, `npm` will reference this list every time when figuring out what to install.

`__npm install [package-name] --save__`

Run this command to install a new package, or piece of software, to be used when creating your site, where `__[package-name]__` is the name of the package you're installing. E.g. `npm install slick.js --save`.

The `--save` flag tells npm to add your piece of software to the list of dependencies in the `package.json` file. That way, when you decide to work on your project somewhere else, then running `npm install` will include this new package you've installed in the list of software it installs.

### Note: the node_modules folder

When you install node modules with npm, they are installed to the present working directory (the one in which you're running the command). The packages and modules that npm installs are installed to a directory called _node_modules_. It's important to note that we will never check this folder in to Git. That said, don't worry when you check in your project and you don't see the node_modules folder. For this class, I've included a file called `.gitignore` in your projectso that will tell GitHub to not commit this folder.

It's a bad idea to commit this folder for two reasons:

- It's huge.
        - Whenever you install packages, each package usually has a set of dependencies, and those can have dependencies, and so forth. And so, as a lot of dependencies are installed, they tend to take up way more space than needed for your _actual_ working files.
- Assume that the files in node_modules are off limits.
        - Even though you've downloaded all these packages with npm, the point is that they're there for you to use with your projects, but _never_ change of the files in this folder yourself becuase the authors of these packages have made them in such a way that they will perform the same for everyone that uses them. We'll review more about this concept in class.
- npm will always recereate this folder for you
        - When you go home and clone your project, then run `npm install`, npm will use `package.json` to recreate this folder for you anyway. That's less for you to keep track of.

## Gulp

We will review more on the concept of gulp in the next class.

