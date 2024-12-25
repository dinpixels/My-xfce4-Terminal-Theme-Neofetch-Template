# My xfce4 Terminal Theme & Neofetch Template
Uses oh-my-posh and applies the catppuccin theme to the xfce4 terminal.  
This template can be copy-pasted to user's directory assuming they already have oh-my-posh installed.

![preview](/preview.png)

**WARNING!** This will completely replace what settings you have for your own terminal.  
I have nothing to do if anything breaks in your end. Proceed only if you know what you're doing.

## Table of Contents
- [Quick Guide](#quick%20guide)
- [Formatting](#formatting)
- [ASCII Art](#ascii%20art)
- [Dependencies](#dependencies)
- [Tools](#tools)
- [To-do](#to-do)

## Quick guide
- Install oh-my-posh (see [this guide](https://calebschoepp.com/blog/2021/how-to-setup-oh-my-posh-on-ubuntu/))
- Download this template
- After following the guide and the installation, copy this template's files to the user directory `${HOME}`
- Done! With that the changes should be applied when running a new terminal instance.

## Formatting
Most stuff here are hand-coded and **are static** as I didn't liked how limited the original formatting.  
There's an exception, the weather info is requested from [wttr.in](https://wttr.in) via `curl`.

Thanks to `.bashrc` and `config.conf` setup, just entering the `neofetch` command alone renders all these info. To add more info, simply edit the `config.conf`.

## ASCII Art
It is loaded from `ascii.txt` through `image_source="${HOME}/.config/neofetch/ascii.txt"` in `config.conf`.

I used [ASCII-Generator](https://ascii-generator.site/) to convert my pixel art into ASCII, and I hand-drawn other characters to
adjust the ASCII art properly.  
To make the colors work correctly, the ASCII art is inverted in color. Overall, the process is just a matter of trial and error.

**Why use a custom ASCII?** To have more control to the ASCII art. Additionally, it's because that the image backend is just a hack as [stated by the maintainer of neofetch](https://github.com/dylanaraps/neofetch/issues/1392#issue-553838221), thus having many issues when rendering images.

## Dependencies
- **xfce4 terminal** - [https://gitlab.xfce.org/apps/xfce4-terminal](https://gitlab.xfce.org/apps/xfce4-terminal), for the awesome terminal
- **oh my posh** - [https://github.com/JanDeDobbeleer/oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh), to prettify the terminal

## Tools
- **Aseprite** - [https://www.aseprite.org/](https://www.aseprite.org/), for drawing pixel art
- **ASCII-Generator** - [https://ascii-generator.site/](https://ascii-generator.site/), for image-to-ASCII conversion
- **Neofetch** - [https://github.com/dylanaraps/neofetch](https://github.com/dylanaraps/neofetch), for displaying system info and more in terminal

## To-do
- [x] Add neofetch config
- [ ] Add VSCodium config
- [ ] Setup script
- [ ] Add a tutorial for making a colored ASCII art