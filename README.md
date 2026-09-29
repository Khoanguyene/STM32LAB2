# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 3

The four-digit scanning logic is reorganized around `update7SEG(int index)` and a four-element `led_buffer`. TIM2 selects the next display every 500 ms, while the DOT LEDs controlled by PA4 toggle every second.

- TIM2 interrupt period: 10 ms
- Full scanning period: 2 s
- Full scanning frequency: 0.5 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

The default test buffer is `{1, 2, 3, 4}`. The `Ex3` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
