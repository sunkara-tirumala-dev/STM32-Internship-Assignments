# STM32 ADC Sensor Reading with UART Output and LED Control

##  Description
This project demonstrates Analog-to-Digital Conversion (ADC) using STM32F401RE. The analog input from a sensor is converted into a digital value, displayed via UART, and used to control an LED.

##  Objective
To implement ADC data acquisition and use the digital output for real-time monitoring and control.

##  Components Used
- STM32F401RE
- Potentiometer / Analog Sensor
- LED

##  Software Used
- Proteus (for simulation)
- Code Composer Studio
- Embedded C

##  Working Principle
- Analog signal is applied to PA1 (ADC channel 1)
- ADC converts analog signal into digital value (0–4095)
- The value is printed via UART using `printf`
- If ADC value exceeds threshold (2000):
  - LED turns ON
- Otherwise:
  - LED turns OFF

##  Features
- Continuous ADC conversion
- UART data transmission
- Real-time LED control
- Register-level programming

##  Code Explanation

### ADC
- PA1 configured as analog input
- ADC1 enabled and configured
- Continuous conversion mode enabled
- Digital value read from ADC_DR

### UART
- USART2 initialized at 115200 baud rate
- `printf` redirected to UART using `__io_putchar`

### GPIO
- PA5 configured as output (LED)
- BSRR used for efficient LED control

### Logic
- Read ADC value
- Print value via UART
- Compare with threshold (2000)
- Control LED accordingly

##  Output
Example UART Output:
Sensor Value: 1023  
Sensor Value: 2048  
Sensor Value: 3500  

- LED turns ON when value > 2000
- LED turns OFF when value ≤ 2000

##  Demo Video
https://drive.google.com/file/d/1jypWmX5YgDA4DIqArHLaivuAn2FfRWcV/view?usp=drive_link

##  Learning Outcome
- ADC configuration and usage
- UART communication with printf
- Sensor interfacing
- Embedded system integration

##  Applications
- Sensor monitoring systems
- Temperature/light control systems
- Embedded automation
