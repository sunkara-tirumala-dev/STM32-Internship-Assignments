# STM32 GPIO Output Control using BSRR (LED Blinking)

##  Description
This project demonstrates GPIO output control using the BSRR (Bit Set Reset Register) in STM32F401RE. An LED is turned ON and OFF continuously using register-level programming.

##  Objective
To control a GPIO output pin efficiently using the BSRR register and understand low-level register manipulation.

##  Components Used
- STM32F401RE
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- GPIOA pin PA5 is configured as output.
- The LED is connected to PA5.
- The BSRR register is used to:
  - Set the pin HIGH (LED ON)
  - Reset the pin LOW (LED OFF)
- A delay loop is used to create visible blinking.

##  Features
- Fast GPIO control using BSRR
- Atomic set/reset operation
- Simple LED blinking implementation

##  Code Explanation
- Enable GPIOA clock using RCC->AHB1ENR
- Configure PA5 as output using MODER register

- BSRR register usage:
  - GPIOA->BSRR = (1 << 5) → LED ON
  - GPIOA->BSRR = (1 << 21) → LED OFF

- Infinite loop toggles LED with delay

##  Output
- LED blinks continuously
- ON and OFF states visible with delay

##  Demo Video
https://drive.google.com/file/d/1z_jxhVn-i9Jh7XEbD5fTBtzjY_Tweeak/view?usp=drive_link

##  Learning Outcome
- Understanding GPIO output configuration
- Use of BSRR register for efficient control
- Basic delay generation using loops

##  Applications
- LED blinking systems
- Status indicators
- Embedded system debugging
