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
    echo "export PATH=$PATH:$HOME/.npm-global/bin"
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



## npm – Node Package Manager

TBD

## Gulp

TBD

## Sass

TBD
