# Intro to Vim

## Why even use vim?

Vim is a powerful text editor that comes pre-installed on most UNIX machines. Desktop operating systems allow you to use familiar, graphical text editors, but you may run into situations where that option isn't available. For example, if you're doing work on a more lightweight device \(like a Raspberry Pi\), or working with servers that you don't physically own, vim might be the only way to edit your files.

## Setting up vim

Vim's default settings are very minimal and aren't ideal for writing C++ code. Let's fix that by changing some of the settings!

Vim's settings are located in a file called `.vimrc` in your home directory, which you can edit by running the command `vim ~/.vimrc`.

Make sure you are in insert mode by pressing `i` on your keyboard. Once you are in insert mode, you should see the text `-- INSERT --` at the bottom of your screen. Copy/paste or manually type the following lines into the file:

{% code-tabs %}
{% code-tabs-item title="~/.vimrc" %}
```text
set nocompatible
set number
syntax on
set autoindent
set cindent
set backspace=indent,eol,start
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Exit insert mode by pressing the Escape key on your keyboard, then type `:wq` and press enter to save the file.

If you did everything correctly, the next time you open vim, you should have syntax highlighting and line numbers enabled, which will be very useful for editing C++ code!

## How much vim do I _need_ to know?

There are a few things you need to know in order to survive in vim.

### 1. The escape key

Vim can be very picky about what keys you press and in what order you press them. If you accidentally press the wrong key, chances are vim will do something that you didn't expect to happen. If this happens to you, hitting escape will bring you back to "normal" mode.

### 2. Normal mode vs. Insert mode

Vim's default mode is "normal" mode. In this mode, every key on your keyboard corresponds to a specific action \(such as copy/paste, search, save, etc.\)

When you want to actually start writing code, you'll need to enter "insert" mode. You can do this by pressing `i` while you are in insert mode. In insert mode, anything you type will be inserted into the file. Pressing escape will exit "insert" mode and bring you back to "normal" mode?

### 3. Saving and Quitting

In order to save, you must start off in "normal" mode. Press escape to get there if you haven't.

Press `:` to enter command-line mode. You should see your cursor move to the bottom of the window.

Type `wq` and press enter to save the file. The `w` means "write" \(as in "write to file", i.e. "save"\) and the `q` means "quit".

{% hint style="warning" %}
#### I'm getting an error saying "No file name"!

If you're getting this error, it's because you opened vim without specifying the file you wanted to open/create in the terminal. That means you did something like `vim` instead of `vim main.cpp`.

If this happens to you, you can specify the filename you want to save the file as after the `wq`. For example, if you wanted to save the file as "main.cpp", you would type `:wq main.cpp` and press enter.
{% endhint %}

