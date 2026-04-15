# STM32 EXTI (External Interrupt)

##  Description
This project demonstrates External Interrupt (EXTI) using STM32F401RE. An interrupt is triggered when an external event (like a button press) occurs.

##  Objective
To understand and implement external interrupts using STM32 and handle events without continuous polling.

##  Components Used
- STM32F401RE
- Push Button
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
When the push button is pressed, an external interrupt is generated. The microcontroller executes the interrupt service routine (ISR), which toggles the LED.

##  Features
- Interrupt-based event handling
- No continuous polling required
- Faster response to external signals

##  Output
LED toggles when the button is pressed.

##  Demo Video
https://drive.google.com/file/d/1MSGgtsxQndc0soG_c752CEl8i_Iu56-S/view?usp=drive_link

##  Learning Outcome
- Understanding of interrupts
- EXTI configuration in STM32
- NVIC handling
