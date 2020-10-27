# Recursivesoft Sphere Module Spec
![alt txt](https://raw.githubusercontent.com/recursivesoft02/-Recursivesoft-Sphere-Module-Spec/master/rec/sphare_module.png)
- Dimensions: 33mm x 22mm x 3.5mm
- OTA authentication & updates (device lifetime)
- Onboard dual-band 2.4/5GHz chip antenna
- Operating temperature: - -35C to +85°C

# Table of contents
- [Microsoft Azure Sphere SoC based module solution for advanced end-to-end IOT security ](#Microsoft-Azure-Sphere-Soc-based-module-solution-for-advanced-end-to-end-IOT-security)
- [Module I/O peripheral support](#Module-I/O-peripheral-support)
- [Wi-Fi Subsystem](#Wi-Fi-Subsystem)
- [Wi-Fi Antenna](#Wi-Fi-Antenna)
- [A7 Application Processor](#A7-Application-Processor)
- [M4F IO Processors ](#M4F-IO-Processors)
- [Flash Memory](#Flash-Memory)
- [Pluton Security Subsystem](#Pluton-Security-Subsystem)
- [Real Time Clock (RTC)](#Real-Time-Clock-(RTC))
- [Peripheral Serial Interfaces ](#Peripheral-Serial-Interfaces)
- [Other I/O Interfaces All pinned-out I/O pins (including ISU interfaces listed above) can be -n individually configured as GPIO pins. A subset of these can be configured as](#Other-I/O-Interfaces-All-pinned-out-I/O-pins-(including-ISU-interfaces-listed-above)-can-be-individually-configured-as-GPIO-pins.-A-subset-of-these-can-be-configured-as)
- [Bootstrap Pins](#Bootstrap-Pins)

## Microsoft Azure Sphere SoC based module solution for advanced end-to-end IOT security
- 1x 500MHz Arm Cortex A7 application processor with 4MB SRAM
- 2x 200MHz Arm Cortex M4F cores, each with 64KB SRAM
- 4MB embedded RAM (shared)
- 16MB QSPI flash memory
- Dual-band 2.4/5GHz 802.11 a/b/g/n Wi-Fi 

## Module I/O peripheral support
- 3x ISU interfaces, pre-configured for UART, SPI, I2C
- ADC/GPIO: 12-bit ADC inputs
- PWM/GPIO: PWM outputs
- RTC (requires VBAT supply)
- Programming & recovery interface 

## Wi-Fi Subsystem
- Dual-band 2.4/5GHz 802.11 a/b/g/n Wi-Fi (20 MHz channels only)
- Has an N968 Andes 32bit MCU
- Uses an external 26 MHz crystal oscillator on the module
- Has an integrated 5GHz Balun
- Uses external 2.4GHz Balun and Diplexer devices on the module 

## Wi-Fi Antenna
- The module is fitted with an on-board dual-band chip antenna for 2.4GHz and 5GHz operation
(Pulse Electronics antenna p/n: W3006)
- An inline switched RF probe connector is provided to facilitated RF conducted measurements 

## A7 Application Processor
- 1x 500MHz Arm Cortex A7 application processor core, with 4MB SRAM (shared)

## M4F IO Processors 
- 2x 200MHz Arm Cortex M4F IO processor cores, each with 64KB SRAM
- The module pins-out the IO0_TXD and IO1_TXD pins from their dedicated UARTs
- SWD interface based debug and programming of M4F IO MCU cores may at later date be enabled 

## Flash Memory 
- 16MB 100MHz (on-die) QSPI flash memory 

## Pluton Security Subsystem
-1x Cortex M4F MCU, dedicated RAM, ROM and GP timers, system control outputs

## Real Time Clock (RTC)
- Low-power RTC with timer/time of day control over system power (32KHz crystal oscillator) 

## Peripheral Serial Interfaces 
- Three ISU serial interfaces are pinned-out. Their accessible pins are limited to that needed for
support of:
- ISU0: UART, max rate=3Mbps (4-wire)
- ISU1: SPI , max rate=40 MHz (5-wire)
- ISU2: I2C , max rate=1MHz (2-wire) 

## Other I/O Interfaces All pinned-out I/O pins (including ISU interfaces listed above) can be individually configured as GPIO pins. A subset of these can be configured as
- PWM outputs
- ADC inputs
- EXT INT inputs

## Bootstrap Pins
![alt txt](https://raw.githubusercontent.com/recursivesoft02/-Recursivesoft-Sphere-Module-Spec/master/rec/BootstrapPins.png)
