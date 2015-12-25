# dottmux

This is my (basic) tmux configuration.

## Installation

Check if tmux is installed:

    tmux -V 

If tmux isn't already installed, install it.
On Os X you typically run:

    brew install tmux

To install this configuration on a new machine:
Make sure you have backed up the .tmux.conf file, because it has to be overridden.
Then run the following commands:

    cd ~
    mkdir .tmux
    git clone git@github.com:Quinten/dottmux.git .tmux
    echo "source-file ~/.tmux/tmux.conf" > ~/.tmux.conf

This repository has submodules. You still need to run:

    cd .tmux
    git submodule init
    git submodule update

If you are already in a tmux session, you can refresh the statusline with:

    tmux source-file ~/.tmux.conf

For the fancy triangles it is recommended to have a powerline font installed. See https://github.com/powerline/fonts

You might also be interested in https://github.com/Quinten/dotvim
