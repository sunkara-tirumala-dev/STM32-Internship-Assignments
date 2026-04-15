# STM32 GPIO Control using CMSIS (LED Blinking)

##  Description
This project demonstrates GPIO control using CMSIS (Cortex Microcontroller Software Interface Standard) in STM32F401RE. An LED is toggled using CMSIS-based register definitions.

##  Objective
To understand how CMSIS simplifies register-level programming by providing structured access to peripheral registers.

##  Components Used
- STM32F401RE
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- CMSIS provides predefined structures for peripheral registers.
- GPIOA is configured as output using CMSIS definitions.
- LED connected to PA5 is toggled continuously using a delay loop.

##  Features
- Easy-to-read code using CMSIS
- Structured register access
- Reduced coding errors compared to raw register access

##  Code Explanation
- CMSIS header `stm32f4xx.h` is included
- GPIOA clock enabled using RCC->AHB1ENR
- PA5 configured as output using MODER register
- LED toggled using:
  - GPIOA->ODR ^= (1 << 5)

- Delay loop used to create blinking effect

##  Output
- LED connected to PA5 blinks continuously

##  Demo Video
https://drive.google.com/file/d/16pk8ZxSmcmsas73mtsuvz5mzITJRA82T/view?usp=drive_link

##  Learning Outcome
- Understanding CMSIS usage
- GPIO configuration using CMSIS
- Embedded C programming basics

##  Applications
- Embedded system development
- Hardware abstraction
- Firmware design
