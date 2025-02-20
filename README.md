# BeebLink

A file storage system for the BBC Micro. Make your PC do something
useful for a change: have it act as a file server for your BBC.

No more swapping discs, no more noisy drives, no more 31 file limit,
file access is very fast, and it's super-easy to share BBC files with
your PC.

If you've got multiple BBCs, they can all connect at once and share
files.

["Action" screen grabs](./docs/screens.md)

# Setting up

Pre-built files are available from
[the BeebLink releases page](https://github.com/tom-seddon/beeblink/releases).
GitHub should highlight the latest release that has files attached -
use that one!

You'll need a PC running Windows, OS X or Linux. If using Windows or
OS X, download the ROMs zip and the appropriate server zip; if using
Linux, download the ROMs zip, and follow
[the building instructions](./docs/build-server.md).

You'll need a BBC B/B+/Master 128, ideally with some kind of EEPROM
module or battery-backed write-protectable sideways RAM - it's no fun
having to reload the ROM each time you power on, or have it zapped by
careless programs!

You can connect BBC and PC using a Tube USB serial adapter
(recommended - it's much faster) or a UPURS cable.

## Tube USB serial adapter

See https://stardot.org.uk/forums/viewtopic.php?f=8&t=14849. You'll
need the full kit with the PLD.

Connect the Tube serial board to the BBC's Tube connector, connect any
second processor to the Tube serial board, use the jumper to select
Comms mode, and connect the device to your PC. If using Windows,
you'll need to
[tweak one of the device settings](./docs/ftdi_latency_timer.md).

If you've got some way of getting files to your BBC already, copy
`beeblink_tube_serial.rom` from the ROMs zip and load it on your BBC;
otherwise, use the [bootstrap process](./docs/bootstrap.md), and get
the file that way.

## UPURS cable _(experimental)_

**UPURS support is experimental**

See https://www.retro-kit.co.uk/UPURS/. Unless your PC is rather old,
you'll also probably need a USB serial port adapter.

If using an FTDI USB to serial adapter on Windows, you'll need to
[tweak one of the device settings](./docs/ftdi_latency_timer.md).

There's no bootstrap process for the UPURS cable - use the UPURS tools
to get `beeblink_upurs_fe60.rom` copied onto your BBC.

[There are some notes about using BeebLink with the UPURS cable](./docs/upurs.md).

**UPURS support is experimental**

# Use

See [the filing system docs](./docs/fs.md) for some info about how to
use it from the BBC side.

[The server docs](./docs/server.md) have some information about useful
command line options, and a few notes about sharing files between BBC
and PC.

[If you use git, some notes on git interop](./docs/git.md).

[Some notes about using BeebLink with the UPURS cable](./docs/upurs.md).

# Building it yourself

[How to build the server](./docs/build-server.md).

[How to build the ROM](./docs/build-rom.md).

# Problems?

Please
[file a GitHub issue](https://github.com/tom-seddon/beeblink/issues)
or
[post in the StarDot BeebLink thread](https://stardot.org.uk/forums/viewtopic.php?f=53&t=15605)
if you run into any difficulties!
