---
title: Shortcuts for Visual Studio Code
date: 2023-05-31 17:37:53 +8:00
categories: [Notes,Visual Studio Code]
tags: [terminal,shortucts,vscode]
---

#### ***The less you rely on the mouse, the better.***

Note: For parameters enclosed in angled brackets, i.e. `<name>`, replace both the word and the brackets with your input.

Do note that many of these commands also apply for the terminal or keyboard in general.

> This doesn't really go anywhere, but it's super helpful:
>
> `CTRL + K + V` previews Markdown files! 
>
> ...do make sure `CTRL` isn't held by the time you press `V` though.
> This is because `CTRL + K` is a "chord" which expects another key afterwards.

## Basic Commands

`code <file>`

* Creates and/or opens a specified file.

* If the file doesn't exist, it is created then opened.

* If the file exists, it is opened.

```bash
# 1.) Opens current directory
code .

# 2.) opens it:
code <filename>.<extension>

# 3.) Example of #2:
code hi_mom.c
```

<!-- Need the double backticks AND the trailing whitespace... ok -->

``CTRL + ` ``

* Opens/Hides the terminal window.

* Uses your Default Shell, like PowerShell or Bash.

* If running multiple terminals, make sure to label them!

`CTRL + P`

* Opens the Command Palete.

* By default lets you search for files in your current workspace and then open them. 

* Type `>` to run a command, both for VS Code itself or installed extensions.

* Type `@` to search for symbols within your current file.

* Type `#` to search for a symbol throughout the entire project including dependencies. If your symbol name is super long, just type its camelCase initials!

* Type `:` and then some number to focus on a particular line.

`CTRL + SHIFT + .`

* Runs the search for symbols command within your file without needing to open up the command palette.

`UP/DOWN`

* When in the terminal, it cycles through your command history.

* When coding, it simply moves your cursor up or down a line.

#### *Remember, you can use the arrowkeys for a lot of things!*

## Character/Word Selection

`SHIFT + ARROW-KEYS`

* Highlights one character at a time (`LEFT/RIGHT`) or line-by-line (`UP/DOWN`).

`CTRL + LEFT/RIGHT`

* Moves your cursor word by word.

`CTRL + D`

* Selects the nearest word. 

* Repeat this command to select multiple instances of that word.

## Line Editing

`ALT + CLICK`

* Sets multiple cursors at the point/s you click.

* Can be done for as many cursors as you like.

`CTRL + G + <line-number>`

* Focus on a particular line.

`CTRL + L`

* Highlights the current line/s.

`CTRL + /`

* Toggles comments on/off for the current line/s.

`CTRL + X`

* Cuts an entire line/s at the point/s your cursor is currently at.

`CTRL + UP/DOWN`

* Moves your field of view up or down line-by-line.

`ALT + UP/DOWN`

* Quickly moves a line up or down.

`ALT + SHIFT + UP/DOWN`

* Quickly copies the current line downwards.


