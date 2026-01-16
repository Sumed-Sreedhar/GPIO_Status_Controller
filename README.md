GPIO-Driven Status Controller (STM32)
Overview:

*This project implements a basic GPIO status controller on the STM32F446RE to understand how inputs, outputs, polling, debouncing, and interrupts work at a fundamental level.

*The project was designed as a foundational embedded systems exercise before moving to fully event-driven architectures.


Hardware Used:

*STM32F446RE (Nucleo)

*Push button(s)

*LED(s)

*On-board ST-Link debugger


Core Concepts Demonstrated:

*GPIO input and output configuration

*Polling vs interrupt-based input handling

*Software debouncing

*Basic timer usage

*Interrupt flow and callbacks

*Understanding hardware vs software responsibilities


System Behavior:

*Button input is read using polling and/or EXTI interrupts

*Button presses change the LED status

*Debouncing logic is applied to avoid false triggers

*LED behavior is controlled directly based on input conditions

*This project focuses on correct signal handling, not advanced state abstraction.


Design Intent:-

The goal of this project was to:

*Build confidence with STM32 GPIO configuration

*Understand how polling differs from interrupts

*Learn how debouncing works in practice

*Observe interrupt execution and callback behavior

*Create a working hardware-validated system

*This project intentionally keeps logic simple to avoid premature abstraction.


What I Learned:

*How GPIO inputs behave electrically

*Why debouncing is necessary

*How EXTI interrupts are triggered and handled

*The difference between polling loops and interrupt-driven logic

*How STM32 HAL structures initialization and callbacks


Limitations:

*Logic is tightly coupled to input handling

*LED control occurs directly in response to inputs

*Not scalable for complex behaviors

These limitations were intentional and later addressed in follow-up projects.


Follow-Up Work:

This project served as the foundation for:

*Event-driven LED controller using EXTI + timers

*Proper state machine–based designs

*Single-point hardware control architectures


Tools & Environment:

*STM32CubeIDE

*STM32 HAL

*Linux (development environment)

*Git & GitHub for version control


Status:
Completed and tested on hardware.
