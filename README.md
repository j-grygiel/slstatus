# slstatus - suckless status
slstatus is a suckless status monitor for window managers that use WM_NAME (e.g. dwm) or stdin to fill the status bar.


## Features
### Used in my Setup
- CPU usage
- Custom shell commands
    - [Volume Indicator](https://github.com/j-grygiel/dotfiles/blob/master/scripts/sb-volume)
- Date and time
- Network speeds (RX and TX)
- Temperature
### Not Used in my Setup
- Battery percentage/state/time left
- Cat (read file)
- CPU frequency
- Disk status (free storage, percentage, total storage and used storage)
- Available entropy
- Username/GID/UID
- Hostname
- IP address (IPv4 and IPv6)
- Kernel version
- Keyboard indicators
- Keymap
- Load average
- Number of files in a directory (hint: Maildir)
- Memory status (free memory, percentage, total memory and used memory)
- Swap status (free swap, percentage, total swap and used swap)
- Uptime
- Volume percentage
- WiFi signal percentage and ESSID


## Requirements
Currently slstatus works on FreeBSD, Linux and OpenBSD.
In order to build slstatus you need the Xlib header files.

- For volume percentage on Linux the kernel module `snd-mixer-oss` must be loaded.
- For volume percentage on FreeBSD, `sndio` must be installed.


## Installation
Edit config.mk to match your local setup (slstatus is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install slstatus (if necessary as root):

`make clean install`


## Running slstatus
See the man page for details.


## Configuration
slstatus can be customized by creating a custom config.h and (re)compiling the source code. This keeps it fast, secure and simple.
