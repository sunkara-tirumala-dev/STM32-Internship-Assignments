# STM32 UART Communication with Button Control

##  Description
This project demonstrates UART communication using STM32F401RE. A push button is used to transmit data, and the received data is used to control an LED.

##  Objective
To implement UART transmission and reception using register-level programming and control peripherals based on received data.

##  Components Used
- STM32F401RE
- Push Button
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- USART2 is configured for UART communication at 9600 baud rate.
- PA2 → TX (Transmit)
- PA3 → RX (Receive)
- PC13 → Push Button input
- PA5 → LED output

- When the button is pressed:
  - Character '1' is transmitted via UART

- When data is received:
  - If received data is '1'
  - LED toggles ON/OFF

##  Features
- UART Transmit and Receive
- Interrupt-free polling method
- Real-time control using UART
- Button-triggered communication

##  Code Explanation
- GPIOA and GPIOC clocks are enabled
- PA2 and PA3 configured for alternate function (UART)
- USART2 configured with:
  - Baud rate = 9600
  - Transmit and Receive enabled

- Button connected to PC13:
  - Detects falling edge (press)

- UART Functions:
  - uart_write() → sends data
  - uart_read() → receives data

- Logic:
  - Button press → send '1'
  - If '1' received → toggle LED

##  Output
- Press button → data transmitted ('1')
- Receiving '1' → LED toggles

##  Demo Video
https://drive.google.com/file/d/1xNlq4YSH9AWZ0mJ-j_ardUGB7ym2GrYT/view?usp=drive_link

##  Learning Outcome
- UART communication (TX & RX)
- GPIO input/output handling
- Serial communication basics
- Register-level peripheral control

##  Applications
- Serial communication systems
- Remote device control
- Embedded communication interfaces
