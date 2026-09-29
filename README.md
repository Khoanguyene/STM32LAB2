# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 8

All display processing is moved to the non-blocking main loop. `timer0` updates the clock and DOT LEDs every second, while a second software timer invokes `update7SEG()` every 250 ms.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

The TIM2 callback now only calls `timer_run()`, keeping the interrupt handler minimal. The `Ex8` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
