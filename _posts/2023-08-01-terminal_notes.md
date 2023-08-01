---
title: General Shortcuts/Commands
date: 2023-08-01 14:58:43 +8:00
categories: [Notes,Miscellaneous]
tags: [terminal,shortucts,windows,keyboard]
---

Note: I'm on **Windows 10.**

Paths in this document are the default installations on this platform.

## Keyboard

### Navigation

`CTRL + LEFT/RIGHT`

* Moves the cursor 1 word to the left or right.

`CTRL + UP/DOWN`

* Shifts your current view 1 line above or below.

### Word Selection

`SHIFT + LEFT/RIGHT`
* Highlights and selects 1 character to the left or right.

`SHIFT + UP/DOWN`
* Highlights and selects the current position up to a certain point (usually a whitespace) in the line above or below.

`CTRL + SHIFT + LEFT/RIGHT`

* Highlights the "word" to the left or right.

### Word Manipulation

`CTRL + BACKSPACE`

* Quickly deletes 1 word to the left.

`CTRL + DELETE`

* Quickly deletes 1 word to the right.

<hr>

## Windows Command Prompt 

### Location 

`C:\WINDOWS\system32\cmd.exe`

This is generally where it's but here's a few other ways you can access it:

1. `WINKEY` + `S`.

    This will open the Search Bar. You can also just open the Search Bar manually via the Start Menu.

    Type `cmd` or `command`. 

    The option for *Command Prompt* should pop up. 
    
    Press `ENTER` or left-click to open. 

2. `WINKEY` + `R`

    Opens the `Run` program which you can use, to well, run things.

    Type `cmd` and press `ENTER` to open *Command Prompt*.

## **(Everything after this is under construction.)**

## Windows PowerShell 

`powershell.exe`

1. `WINKEY + S`

    Type `ps` or `powershell`.
    
    Press `ENTER` or left-click the icon to open.

2. `WINKEY + X`

    Open the *Quick Link Menu*.

    Navigate using the `UP/DOWN` arrowkeys and press `ENTER` when you see *Windows Powershell* is highlighted. 

    You can also open *Windows Powershell (Admin)* if you're doing something that requires Admin privileges.

### Basic Commands

Many of these are common across different shells, but some are Windows specific.

`help`
* When in doubt, this will be your friend!


`exit`

`cd`

`cls`

`dir`

`echo`

`mv`

`mkdir`

`rm`

`set`

`setx`

`xcopy`

### Shortcuts

`CTRL + C`

Cancels writing the current command but does not erase your input, immediately moves the cursor to a new line.

Useful if you wrote a long command and decided you don't want to run it.

`UP/DOWN`

Cycles through your recent command history for the current session.

---

## MSYS2 UCRT64

`C:\msys64\ucrt64.exe`

The package manager is known as `pacman`.

Usage:
```shell
pacman -S [options] [package(s)]
```

`-S` is shorthand for `--sync`. Common options are:
```
-y, --refresh       Download fresh package databases from a server.
                    (-yy to force a refresh even if up to date)

-u, --sysupgrade    Upgrade installed packages.
                    (-uu enables downgrades)
```

---

## FFMPEG

Usage:

```
ffmpeg -i <file>.<ext> <out>.<ext>

Basic options/arugments:

-i              Specifies that the next argument is the input file.
<file>.<ext>    The input's filename with its original extension.
<out>.<ext>     The desired output name with the desired format extension.
```

Example:

```
ffmpeg -i family_video.mov family_video.mp4

This will take my input file "family_video.mov" and convert it to a .mp4 file with the same name.
```

Some useful options:

```
Placed before -i:

-ss <HH:MM:SS.MS>   Seeks the given timestamp to start encoding at.


Placed after -i:

-vcodec <codec>     Sets the output encoding format using the next arugment.
                    e.g. ffmpeg -i family_video.mov -vcodec h264 family_video.mp4

-crf <rate>         Sets the output compression rate using the next argument.
                    e.g. ffmpeg -i family_video.mov -crf 24 family_video.mp4 
                    
-to <HH:MM:SS.MS>   Specifies a timestamp to end encoding at.
-t <num>            Specifies the intended duration of the clip to be encoded.
```
