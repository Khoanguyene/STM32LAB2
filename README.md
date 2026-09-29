# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 2

Four common-anode seven-segment displays are multiplexed by TIM2 interrupts to show `12:30`. Each digit is selected for 500 ms, while two DOT LEDs controlled by PA4 toggle every second.

- TIM2 interrupt period: 10 ms
- Full scanning period: 2 s
- Full scanning frequency: 0.5 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

The `Ex2` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
