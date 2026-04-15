# STM32 GPIO Control using BSRR with Button Input

##  Description
This project demonstrates GPIO input and output control using STM32F401RE. An LED is controlled based on the state of a push button using register-level programming.

##  Objective
To implement GPIO input and output operations using:
- IDR (Input Data Register) for button input
- BSRR (Bit Set Reset Register) for LED control

##  Components Used
- STM32F401RE
- Push Button
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- The push button is connected to GPIOC pin (PC13) as input.
- The LED is connected to GPIOA pin (PA5) as output.
- When the button is pressed, the input pin reads LOW.
- The microcontroller detects this and turns ON the LED.
- When the button is released, the LED turns OFF.

##  Features
- Direct register-level programming
- Efficient GPIO control using BSRR
- Real-time input-output operation

##  Code Explanation
- GPIOA clock is enabled for LED control
- PA5 is configured as output
- GPIOC clock is enabled for button input
- PC13 is configured as input

- BSRR register is used:
  - Lower 16 bits → Set LED (ON)
  - Upper 16 bits → Reset LED (OFF)

- IDR register is used to read button state

- Logic:
  - Button pressed → LED ON
  - Button released → LED OFF

##  Output
- LED turns ON when button is pressed
- LED turns OFF when button is released

##  Demo Video
https://drive.google.com/file/d/17Gek3D_u7qjTFc1K8PoPvUXpO38Iog65/view?usp=drive_link

##  Learning Outcome
- Understanding GPIO input/output
- Usage of IDR and BSRR registers
- Bitwise operations in embedded C

##  Applications
- Button-controlled devices
- Embedded control systems
- Real-time input-based automation
