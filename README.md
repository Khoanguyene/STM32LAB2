# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 5

A digital clock displays hour and minute in `HH:MM` format. The initial time is 15:08:50, `updateClockBuffer()` splits hour and minute into four digits, and the main loop updates time once per second.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

TIM2 continues to scan the display at 1 Hz and toggle the DOT LEDs every second. The `Ex5` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
