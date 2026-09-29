# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 4

The four-digit scanning frequency is increased to 1 Hz. TIM2 selects the next display every 250 ms, while the DOT LEDs controlled by PA4 continue to toggle every second.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

The default test buffer is `{1, 2, 3, 4}`. The `Ex4` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
