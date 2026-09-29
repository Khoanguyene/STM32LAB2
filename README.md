# STM32LAB2

Microprocessors and Microcontrollers - Lab 2: Timer Interrupt and LED Scanning.

## Exercise 6

A 10 ms software timer is added to the digital clock. `timer_run()` decrements the counter from the TIM2 callback, and `timer0_flag` signals expiration to the main loop.

- TIM2 interrupt period: 10 ms
- Full scanning period: 1 s
- Full scanning frequency: 1 Hz
- Microcontroller: STM32F103C6
- Segment outputs: PB0-PB6
- Display enables: PA5-PA8 through PNP transistors
- DOT output: PA4

The Exercise 5 clock behavior and `HAL_Delay(1000)` are retained as required; the software timer prepares the non-blocking implementation in Exercise 7. The `Ex6` branch contains the STM32CubeIDE source, Proteus project, and compiled HEX firmware.
