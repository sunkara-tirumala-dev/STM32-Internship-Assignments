# STM32 Register Manipulation

##  Description
This project demonstrates direct register-level programming using STM32F401RE. The peripheral registers are accessed manually using their memory addresses without using higher-level abstractions.

##  Objective
To understand low-level programming by directly configuring hardware registers for controlling peripherals.

##  Components Used
- STM32F401RE
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
In register manipulation, the microcontroller peripherals are controlled by directly writing to specific memory-mapped registers. For example, GPIO registers are configured to set pin direction and control output.

##  Features
- Direct hardware control
- Faster execution
- No dependency on libraries

##  Output
LED blinks by directly controlling GPIO registers.

##  Demo Video
https://drive.google.com/file/d/1IDofBi-UlB6ac0wbtGNfv6xYfOfNwZNZ/view?usp=drive_link

##  Learning Outcome
- Understanding of memory-mapped registers
- Low-level hardware control
- Bitwise operations in embedded C
