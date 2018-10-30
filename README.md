# ags-snap

[![Snap Status](https://build.snapcraft.io/badge/ericoporto/ags-snap.svg)](https://build.snapcraft.io/user/ericoporto/ags-snap) 
[![Build Status](https://travis-ci.com/ericoporto/ags-snap.svg?branch=master)](https://travis-ci.com/ericoporto/ags-snap)

snap for ags engine for playing games made in Adventure Game Studio on Linux 
(license of snap code is not the license of ags).

Plugins are not supported by this distribution.

## Install

You can install from [snap listing](https://snapcraft.io/ags):

    snap install ags

Alternatively, you can clone this repo and build and install yourself

    git clone git@github.com:ericoporto/ags-snap.git
    snapcraft
    snap install ags_*.snap --dangerous

To unninstal it, use remove

    snap remove ags

## Usage

After installation, you can run it by typing **`ags`** in a directory containing either a 
`game.ags` or a `game.exe`, made in AGS. In some computers, ags runs better using windowed
with `ags --windowed`.

    ags [OPTIONS] [GAMEFILE or DIRECTORY]

    Options:
      --windowed                   Force display mode to windowed
      --fullscreen                 Force display mode to fullscreen
      --hicolor                    Downmix 32bit colors to 16bit
      --gfxfilter <filter> [<scaling>]
                                   Request graphics filter. Available options:
                                     none, stdscale, hqx;
                                     scaling is specified by integer number
      --log                        Enable program output to the log file
      --no-log                     Disable program output to the log file,
                                     overriding configuration file setting
      --help                       Print this help message

    Gamefile options:
      /dir/path/game/              Launch the game in specified directory
      /dir/path/game/penguin.exe   Launch penguin.exe
      [nothing]                    Launch the game in the current directory

