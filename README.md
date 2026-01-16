# GPIO-Driven Status Controller (STM32)

**Status:** Completed and tested on hardware | STM32F446RE

---

## What It Does
A **foundational GPIO control project** built to understand how **inputs, outputs, polling, debouncing, and interrupts** work at a fundamental level on the STM32 platform.

- Reads button input using polling and/or EXTI interrupts  
- Controls LED output directly based on input conditions  
- Applies software debouncing to prevent false triggers  

This project was intentionally designed as a **learning baseline** before transitioning to fully event-driven and state-based architectures.

---

## Hardware Used
- **MCU:** STM32F446RE (Nucleo)
- **Inputs:** Push button(s)
- **Outputs:** LED(s)
- **Debug:** On-board ST-Link debugger

---

## Core Concepts Demonstrated
- GPIO input and output configuration  
- Polling vs interrupt-based input handling  
- Software debouncing techniques  
- Basic timer usage  
- Interrupt flow and callback execution  
- Hardware vs software responsibility separation  

---

## System Behavior
- Button input is read using **polling and/or EXTI interrupts**
- Button presses directly change the **LED state**
- Debouncing logic is applied to avoid false triggers
- Output behavior is controlled immediately in response to inputs

This project focuses on **correct signal handling and reliability**, not architectural abstraction.

---

## Design Intent
The goal of this project was to:

- Build confidence with STM32 GPIO configuration  
- Understand practical differences between polling and interrupts  
- Learn how debouncing works in real hardware  
- Observe interrupt execution and callback behavior  
- Create a working, hardware-validated embedded system  

Logic was intentionally kept simple to avoid premature abstraction.

---

## What I Learned
- How GPIO inputs behave electrically  
- Why debouncing is necessary in real systems  
- How EXTI interrupts are triggered and handled  
- The difference between polling loops and interrupt-driven logic  
- How STM32 HAL structures initialization and callbacks  

---

## Limitations
- Logic is tightly coupled to input handling  
- LED control occurs directly in response to inputs  
- Not scalable for complex or multi-mode behaviors  

These limitations were **intentional** and later addressed in follow-up projects.

---

## Follow-Up Work
This project served as the foundation for:

- Event-driven LED controller using EXTI + timers  
- Proper state machine–based designs  
- Single-point hardware control architectures  

---

## Tools & Environment
- STM32CubeIDE  
- STM32 HAL  
- Linux development environment  
- Git & GitHub for version control  

---

## Status
Completed and tested on hardware.
