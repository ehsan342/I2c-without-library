# I2c-without-library
# I2C Communication with 1602A LCD and Stepper Motor Control - Arduino Uno

This project demonstrates how to establish I2C communication between an Arduino Uno and a 1602A LCD display, along with controlling a stepper motor. The code provided here utilizes direct control without relying on any external libraries.

## Features

- I2C communication with 1602A LCD with backpack pcf8574: Display custom messages on a 16x2 LCD using I2C communication.
- Stepper motor control : Control the speed and direction of a stepper motor using the Arduino Uno.

## Getting Started

### Hardware Requirements

- Arduino Uno
- 1602A LCD Display
- Stepper Motor
- Stepper Motor Driver (e.g., A4988)
- Breadboard and jumper wires

### Wiring Instructions

- Connect the 1602A LCD to the Arduino Uno using I2C:
  - Connect SDA on the LCD to 4 on the Arduino.
  - Connect SCL on the LCD to 5 on the Arduino.

- Connect the stepper motor to the stepper motor driver and then to the Arduino Uno:
  - Connect the step pin of the driver to a digital pin on the Arduino (e.g., 9).
  - Connect the direction pin of the driver to another digital pin on the Arduino (e.g., 8).
  - Power the motor driver with an appropriate power supply.
  - Connect the stepper motor to the motor driver.

### Running the Code

1. Open the Arduino IDE and create a new sketch.
2. Copy and paste the code from the provided `main.ino` file into the sketch.
3. Modify the code as needed (e.g., adjusting pins, motor parameters).
4. Upload the sketch to your Arduino Uno.
5. Observe the LCD displaying messages and the stepper motor responding to commands.

## Code Explanation

- `setup()`: Initializes the I2C communication and sets up the pins for the stepper motor control.
- `loop()`: Contains the main logic for displaying messages on the LCD and controlling the stepper motor.

## Troubleshooting

- If the LCD doesn't display correctly, check the wiring and I2C address configuration.
- If the stepper motor doesn't respond, verify the motor driver wiring and pin configurations.


