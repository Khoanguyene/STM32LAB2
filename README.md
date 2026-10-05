# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 9

Exercise 9 extends the four-digit digital clock with an 8x8 red LED matrix driven by a ULN2803 transistor array. All processing remains in the non-blocking main loop; the TIM2 interrupt handler only updates the software timers.

- Microcontroller: STM32F103C6
- TIM2 interrupt period: 1 ms
- Seven-segment scan period: 5 ms per digit
- LED-matrix scan period: 2 ms per column
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4
- Matrix row outputs: PB8-PB15
- Matrix column enables: PA0-PA3 and PA9-PA12 through ULN2803
- Matrix output: static character `A`

The `Ex9` branch contains the complete STM32CubeIDE source, Proteus project, and compiled HEX firmware.

## Repository layout

- `SOURCE/`: STM32CubeIDE project source
- `PROTEUS/Ex9.pdsprj`: Proteus simulation
- `FIRMWARE/Ex9.hex`: compiled firmware
