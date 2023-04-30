# st - simple terminal

st is a simple terminal emulator for X which sucks less. It's one of suckless utilities, more info [here](https://st.suckless.org/).

## Patches

As this is my own build, I've added some patches to it.

- [anysize](https://st.suckless.org/patches/anysize/)
- [delkey](https://st.suckless.org/patches/delkey/)
- [scrollback](https://st.suckless.org/patches/scrollback/). Edited: Added st-scrollback-ringbuffer-0.8.5.diff only.
- [gruvbox theme](https://github.com/morhetz/gruvbox)

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```bash
$ make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```bash
$ tic -sx st.info
```

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

