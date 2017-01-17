# Tasty guacamole gets things done!

Here's a list of commands to get you up and running, along with some challenges to make you learn the ropes.

If you're new to Unix and/or Git, you may find the following basic commands useful to navigate around. Use Terminal to first clone the repository locally (`git clone https://github.com/MITEVT/psychic-guacamole`). Then plug in to you computer the development board you were given. Switch directories to the top-level directory with a `Makefile`, and run `make` and `make writeflash` to compile your program and download it to the microcontroller to run!

The [FAQ](https://github.com/MITEVT/opel_EE/wiki/Large-General-FAQ-about-LPC11CX2-X4-Microcontrollers) is also good place to read if you're confused or stuck.

## Unix Cheatsheet:

`.` - current directory
`..` - reference to directory one level up

`cd [directory]` - change current directory
`ls [folder]` - list files
`mkdir [directory name]` - make directory


## Git Cheatsheet:
Pull a repository down from GitHub:

1. Copy clone address link from github.com
2. `git clone <address>`

Set github account information:

`git config --global user.name <name>`
`git config --global user.email <email>`

Refresh repository, pull changes from upstream:
`git pull`

Make a commit:
`git add <files to commit>`
`git commit -m "<commit message>"`

Make a branch:
`git checkout -b <new branch name>` - create a branch
`git checkout <branch name>` - switch to a branch
`git branch` - list current branches

## Three Exercises:
1. Blink Exercise - Make an LED blink on and off by writing a delay function. Debug LEDs are super important!
2. UART Echo Exercise - If you run `make com` after you `make writeflash`, a serial I/O connection over UART/USB is set up with the LPC. After you run `make com`, you can't see any of the characters you type, because the chip isn't sending you any characters. Program the LPC to echo input you type back to your terminal input.
3. CAN Exercise - Make two LPC microcontrollers talk to each other over CAN, a differential pair signaling system. For a brief introduction to CAN, a good start the [Wikipedia article](https://en.wikipedia.org/wiki/CAN_bus). Ask questions as necessary. The [later development boards](https://github.com/MITEVT/opel_11U_devboard) should already have the necessary hardware and pins to facilatate a CAN connection between two boards (e.g. termination resistors, etc.)

