# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 1

Two common-anode seven-segment displays are multiplexed by TIM2 interrupts. The first display shows `1`, the second shows `2`, and the active display changes every 500 ms.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA6 through PNP transistors

The `Ex1` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
