

**Smart-Modular-BT-OBV-IR**

This repository contains the Arduino code for a robot that avoids obstacles using ultrasonic and infrared sensors, and can be controlled remotely via Bluetooth. 

**Features:**

* **Obstacle Avoidance:**
    * Utilizes ultrasonic sensor to detect obstacles in front of the robot.
    * Employs infrared sensor to detect nearby obstacles.
    * Stops and changes direction when obstacles are detected.
* **Remote Control via Bluetooth:**
    * Accepts commands (forward, backward, left, right, stop) through serial communication.
    * Allows for remote control of the robot's movement.

**Hardware:**

* Arduino Uno or compatible board
* AFMotor library compatible motor driver (e.g., Adafruit Motor Shield)
* Two DC motors (one for each wheel)
* Ultrasonic sensor (HC-SR04 or equivalent)
* Infrared sensor (GP2Y0A21Y or equivalent)
* Bluetooth module (HC-05 or equivalent)
* Jumper wires
* Breadboard (optional)
* Power supply (e.g., battery pack)

**Software:**

* Arduino IDE (for code development and uploading)
* AFMotor library (for motor control, download link: [https://www.arduino.cc/reference/en/libraries/adafruit-motor-shield-library/](https://www.arduino.cc/reference/en/libraries/adafruit-motor-shield-library/))

**Wiring:**

* Refer to the specific motor driver and sensor datasheets for detailed wiring instructions. 
* Generally, connect the motors, sensors, and Bluetooth module to the appropriate pins on the Arduino board according to the AFMotor library and sensor specifications.

**Code:**

* The `servo.ino` file contains the Arduino code for the robot's functionality.
* The code includes functions for:
    * Motor control using the AFMotor library
    * Ultrasonic distance measurement
    * Infrared obstacle detection
    * Bluetooth serial communication for receiving commands

**Usage:**

1. **Install Libraries:**
   * Download and install the AFMotor library in the Arduino IDE.

2. **Upload Code:**
   * Open the `servo.ino` file in the Arduino IDE.
   * Select your Arduino board and upload the code.

3. **Connect to Bluetooth:**
   * Pair your Bluetooth device (phone, computer) with the HC-05 module (refer to HC-05 documentation for pairing instructions).

4. **Control the Robot:**
   * Use a serial terminal program (e.g., Serial Monitor in Arduino IDE) or a custom Bluetooth app to send commands (F, B, L, R, S) to control the robot's movement.

**Note:**

* This is a basic implementation and may require adjustments based on your specific hardware setup.
* Consider adding features like:
    * Improved obstacle avoidance logic (e.g., turning corners, navigating complex environments).
    * Sensor calibration for more accurate readings.
    * Feedback mechanisms (e.g., LEDs, sounds) to indicate robot status.

**Disclaimer:**

This code and project are provided for educational and experimental purposes only. The author is not responsible for any damage or injury resulting from the use of this system.


