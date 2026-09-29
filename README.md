# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 7

The digital clock is converted to a non-blocking implementation. `timer0_flag` updates the time and toggles the DOT LEDs from the main loop once per second, with no `HAL_Delay(1000)`.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

TIM2 only advances the software timer and scans the four displays. The `Ex7` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
