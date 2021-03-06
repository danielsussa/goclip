# Terminal Clipboard

![record example](gif/example_complete.gif)

Different from others terminal's clipboard coppiers, this one can copy complex and interminables commands like **tail -f** or outputs that spit multi line texts.

## How to use:

You can use goclip to copy a simple command to the clipboard like this:

    $ date | goclip
    Tue Oct 10 22:55:01 PDT 2021

Or use the pipe to capture complex commands that doesn't generate EOF like this:

    $ tail -f file.txt | goclip
    text output1
    text output2
    text output3
    (...)

Pressing **CTRL+C** in this case will make goclip capture the events and copy to the clipboard.

## Installing:

Copy command bellow:

    wget https://github.com/danielsussa/goclip/releases/latest/download/goclip -P $HOME/bin/ && chmod +x $HOME/bin/goclip

Open a new terminal tab and test it:

    $ date | goclip
    Tue Oct 10 22:55:01 PDT 2021

Simple!

[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
