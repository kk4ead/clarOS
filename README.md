# clarOS

A starter kit for the Texas Instruments Tiva C Series [TM4C123GXL][launchpad]
LaunchPad, containing only software with BSD-compatible licenses and no
"TI Commercial" code. Tested on macOS 10.14.3 with Homebrew, but should work
on any other Unix that supports [Linuxbrew][linuxbrew].

## Getting Started

1. Install Homebrew from <https://brew.sh> if you haven't already.
2. Clone this repository with `git clone git@github.com:kk4ead/claros`.
3. Download and install all dependencies with `cd claros && make deps`.
4. Build the demo project with `make`.
5. Connect a LaunchPad and run `make flash`.
   You should see the LED on the board start cycling through colors.
6. Run `screen /dev/cu.usbmodem* 115200` to connect to UART0. You should
   see "red", "green", "red", "blue", print to the console each time the
   corresponding color is toggled.

## Acknowledgements

Thanks to [Josh Minor][jishminor] and [Sean Kirmani][kirmani] for their
[ee445l-linux][ee445l-linux] tools, and to [Zee Lv][ZeeLivermorium] for his
[zEEware][zEEware] tools.

[launchpad]: http://www.ti.com/tool/EK-TM4C123GXL
[linuxbrew]: http://linuxbrew.sh
[jishminor]: https://github.com/jishminor
[kirmani]: https://github.com/kirmani
[ee445l-linux]: https://github.com/jishminor/ee445l-linux
[ZeeLivermorium]: https://github.com/ZeeLivermorium
[zEEware]: https://github.com/ZeeLivermorium/zEEware
