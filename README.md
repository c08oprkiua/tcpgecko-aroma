# What is this?
This is an unofficial TCPGecko port/rewrite for Aroma. 

**At the time of writing this, this is a work in progress and does not work yet**. 

# How do I use this?
This is a plugin for Aroma. Check to make sure it is enabled in the plugin menu. You will have an option in the plugin menu to use "SD codes", which are codes that are locally stored on the SD card instead of sent from a client.

# Compiling

As stated previously, this project is not done yet. However, I will list the libraries I am using/will use in it, for future reference in case I forget to add this later.

To compile this, you will (probably) need:
* `devkitpro`:
  * `libogc` (I'm gonna work on removing this requirement)
  * `wut`
* `libkernel`

# Feature re-implementation checklist:
Though I tried, I cannot guarantee that everything works, because of what was necessarily changed in porting TCPGecko from the old libraries to the new equivalents. 

* Things related to kernel access may be depreciated and/or redundant to their non-kernel counterparts in the future
* **Old codes are expected to not work due to RAM offsets, so please do not report old codes not working as an issue.**

I am reliant on people testing it and getting back to me on the status of various features. A checklist of what has been reported to work is below. 

Commands:
- [ ] Write 8 bit value
- [ ] Write 16 bit value
- [ ] Write 32 bit value
- [ ] Read memory
- [ ] Read memory with kernel access
- [ ] Validate address range
- [ ] Disassemble range (currently disabled)
- [ ] Disassemble memory
- [ ] Read compressed memory
- [ ] Write with kernel access
- [ ] Read with kernel access 
- [ ] Take a screenshot
- [ ] Upload memory
- [ ] Get the size of data buffer
- [ ] Read a file
- [ ] Read a directory
- [ ] Replace a file
- [ ] "IOSU read file" (currently disabled)
- [ ] Get version hash
- [ ] Get code handler address
- [ ] Read threads
- [ ] Get account identifier
- [ ] Write screen (currently disabled)
- [ ] Follow pointer
- [ ] Get server status
- [ ] Remote procedure call
- [ ] Get symbol
- [ ] Search memory 32
- [ ] Advanced memory search
- [ ] Execute assembly
- [ ] Pause the console
- [ ] Unpause the console
- [ ] See whether the console is paused or not
- [ ] Get server version
- [ ] Get OS version 
- [ ] Set data breakpoint
- [ ] Set instruction breakpoint
- [ ] Toggle breakpoint
- [ ] Remove all breakpoints
- [ ] Get stack trace
- [ ] Poke registers
- [ ] Get entry point address
- [ ] Run kernel copy service
- [ ] Persist assembly
- [ ] Clear assembly


# Credits
## Original TCPGecko credits:
* **dimok** for Homebrew Launcher project engine/base
* **BullyWiiPlaza** for further development of advanced/efficient features
* **wj44** for porting [`pyGecko`](https://github.com/wiiudev/pyGecko) to the Homebrew Launcher and some development
* **Marionumber1** for exploit development and TCP Gecko Installer contributions
* **NWPlayer123** for the `pyGecko` client library
* **Chadderz** for the original `TCP Gecko Installer`
* **Kinnay** for some `DiiBugger` code this project made use of

## aRAMa credits:
* **Maschell** for help on Discord
* **Lulsec2#0064** on Discord, for coming up with the name "aRAMa"

# Help, inquiries, etc.
For help with or questions about JGecko U or the original TCPGecko, join [the JGecko U Discord](https://discord.com/invite/rSRM3RWDq4)

For help with or questions about aRAMa, join [my Discord](https://discord.com/invite/VPHr56hnbQ)