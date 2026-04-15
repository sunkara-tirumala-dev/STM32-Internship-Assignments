# STM32 Structure-Based Register Access (GPIO Control)

##  Description
This project demonstrates structure-based register access in STM32F401RE. Instead of using direct memory addresses, structures are used to map peripheral registers, improving code readability and organization.

##  Objective
To understand how to access and control hardware registers using C structures for better abstraction and maintainability.

##  Components Used
- STM32F401RE
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- Peripheral registers are represented using C structures.
- Base addresses are defined and typecast to structure pointers.
- GPIOA is configured as output.
- LED connected to PA5 is toggled continuously.

##  Features
- Structured register mapping
- Improved code readability
- Easier peripheral handling compared to raw pointers

##  Code Explanation
- GPIO_TypeDef structure defines GPIO registers
- RCC_TypeDef structure defines RCC registers

- Base addresses:
  - RCC → 0x40023800
  - GPIOA → 0x40020000

- Clock is enabled using:
  - RCC->AHB1ENR |= (1 << 0)

- PA5 configured as output:
  - MODER register

- LED toggled using:
  - GPIOA->ODR ^= (1 << 5)

- Delay loop is used for visible blinking

##  Output
- LED connected to PA5 blinks continuously

##  Demo Video
https://drive.google.com/file/d/1k-HK4kT-1Scx7FpXqc-FgLOYRR3y8nGT/view?usp=drive_link

##  Learning Outcome
- Understanding structure-based register access
- Memory-mapped I/O concept
- Low-level embedded programming

##  Applications
- Embedded driver development
- Hardware abstraction
- Firmware design
