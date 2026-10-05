# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 10

Exercise 10 extends the digital clock and 8x8 LED matrix from Exercise 9 with a non-blocking scrolling animation. The character `A` shifts left one column every 200 ms and re-enters from the right after leaving the display.

- Microcontroller: STM32F103C6
- TIM2 interrupt period: 1 ms
- Seven-segment scan period: 5 ms per digit
- LED-matrix scan period: 2 ms per column
- Animation update period: 200 ms
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4
- Matrix row outputs: PB8-PB15
- Matrix column enables: PA0-PA3 and PA9-PA12 through ULN2803

The TIM2 callback only invokes `timer_run()`. Clock updates, seven-segment scanning, matrix scanning, and animation updates are all handled in the main loop using software-timer flags.

## Repository layout

- `SOURCE/`: STM32CubeIDE project source
- `PROTEUS/Ex10.pdsprj`: Proteus simulation
- `FIRMWARE/Ex10.hex`: compiled firmware
