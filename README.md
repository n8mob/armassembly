[YouTube Playlist](https://youtube.com/playlist?list=PL8FGoV_syMtGzCmKBHQli1Q0EQEHispMy&si=YCwEilp7DaZUPNBk) by [Will Thomas](https://github.com/willth7)

[RP2040 Datasheet](rp2040-datasheet.pdf) ([original link](https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf))
[ARM v6-M Architecture Reference Manual](DDI0419E_armv6m_arm.pdf) ([original link](https://datasheets.raspberrypi.com/pico/pico-datasheet.pdf))
[Raspberry Pi Pico Datasheet](pico-datasheet.pdf) ([original link](https://developer.arm.com/documentation/ddi0419/e/))


# 1. [Introduction, Development Environment, and the Bus](https://youtu.be/CH9bc-z2vjQ?si=rXC-AlbCGqppJmtI)


## RP2040 Data-sheet Highlights

ARM Cortex M0+, v6 M, "Thumb" mode 16-bit instructions (instead of 32).


### AMBA Arm Advanced Microcontroller Bus Architecture, 1996


### AHB-Lite Crossbar 4:10

1.  AHB AMBA High-performance Bus (wikipedia)

    address phase and data phase, two bus cycles without a wait state
    access to the target is controlled through a MUX, thereby admitting a single master at a time

2.  AHB-Lite is a single-master subset

3.  Crossbar

    "Crossbar" seems to refer to the electrical topology of cross-bar telephone switching hardware.
    According to the Wikipedia [article on Crossbar Switches](https://en.wikipedia.org/wiki/Crossbar_switch), the originals used literal crossing bars. But later the same "switching topology" was implemented in with solid-state electronics.

4.  4:10

    4 upstream ports
    10 downstream ports


### APB Splitter

Advanced Peripheral Bus


## ARM v6-M Notes

"Thumb mode" is a subset of 16-bit instructions ("half-word")
Where Arm is already a reduced instruction set, thumb is reduced even further.

§A6.7 is an alphabetical list of ARMv6-M Thumb Instructions


## Development Environment

1.  Assembler
    `arm-none-eabi-as`
    I believe this refers to "none" for the OS (since we are running "bare metal") and eabi means "Embedded Application Binary Interface", referring to the binary file format. (I believe one alternative to eabi is elf)


# 2. Subsystem Resets and the GPIO


# 3. Oscillators, Clocks, and the PLL


# 4. SRAM


# 5. Dividers, Spinlocks, and the SIO


# 6. UART


# 7. Boot Sequence and Watchdog


# 8. Bootrom and Flash


# 9. Interrupts and Alarms

