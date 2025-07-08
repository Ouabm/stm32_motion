# stm32_motion
This project is a DEVS-based example running on an STM32H743ZI2 development board. It models a system that turn a LED on and off depending on the detection of an object from the motion sensor.

## Features

- Real-time motion monitoring
- Implemented using the DEVS formalism with Cadmium
- Runs on STM32H743ZI2 using ARM toolchain

## Prerequisites

- STM32H743ZI2 development board connected via USB
- motion sensor properly wired (see installation diagram below)
- Cadmium simulaton installed
- ARM toolchain: `gcc-arm-none-eabi`

## Installation

1. **Install the ARM GCC toolchain**:

```bash
sudo apt install gcc-arm-none-eabi
```
## Wiring and running 
1. **Wirning**:

### PIR motion sensor  (Digital Output)

| Signal | PIR Pin    | STM32 Pin Example | Notes                                  |
|--------|------------|-------------------|--------------------------------------- |
| VCC    | V+         | 5V                | Requires stable 5V supply              |
| GND    | GND        | GND               | Common ground                          |
| OUT    | AO         | PA0               | Digital output connected to ADC input  |


2. **Running**:

```bash
git clone https://github.com/Ouabm/stm32_motion.git
```
  then
```bash
cd stm32_motion/
```
  then
```bash
./build_stm32
```
