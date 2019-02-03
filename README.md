# BeebLink

A file storage system for the BBC Micro. Make your PC do something
useful for a change: have it act as a file server for your BBC. No
more swapping discs, no more noisy drives, no more 31 file limit.

["Action" screen grabs](./docs/screens.md)

I use this as the default filing system for my BBC Master and my BBC
B, and will be improving it over time...

# Requirements

Some self-assembly is required.

* 5V-tolerant AVR-based microcontroller board (used to connect BBC's
  user port and PC's USB port). Supported types so far are the Minimus
  AVR 32K and the SparkFun Pro Micro
* PC running OS X, Windows or Linux
* BBC Micro(s) with some good way of loading the ROM image (i.e., with
  something like EEPROM or write-protected battery-backed sideways
  RAM... it's no fun having to reload it on each boot and/or have it
  zapped by careless programs)

# Installation and setup

Download latest release from
[the BeebLink releases page](https://github.com/tom-seddon/beeblink/releases) -
you'll need the firmware ZIP, and a server ZIP for your OS.

Follow [the setup instructions](./docs/setup.md) to set up the AVR.

You can get [debug serial output](./docs/serial.md) from the AVR.

The [filing system docs](./docs/fs.md) give some notes about running
the server and using the filing system.

[Useful server command line options](./docs/server.md).

[Got multiple BBCs? No problem](./docs/multi.md). 

[If you use git, some notes on git interop](./docs/git.md).

# Building it yourself

**This repo has submodules** - if you're going to build it, clone it
with `git clone --recursive`, or do `git submodule init && git
submodule update` from the working copy after a normal clone.

(If using Linux or 32-bit Windows, follow the instructions here for
running the server. There are no binary releases for these systems.)

[Building instructions](./docs/build.md)
