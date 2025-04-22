# MPU6050 Code for a Gesture-Controlled Room Project

## A code written in the Arduino IDE using C++ for an MPU6050 sensor that controls LEDs, servo motors and a fan

Control lights, fans, servos, and more with hand gestures! This Arduino-based project uses the MPU6050 sensor (with built-in accelerometer and gyroscope) to detect motions like swipes, tilts, and lifts. It is beginner-friendly and perfect for DIY smart home systems, IoT prototypes, or accessibility tech. Unlike voice control, the system can work silently. The code translates sensor data into real-world actions such as, adjusting LEDs, servo-controlled curtains or the fan.

## Features
* Gesture Recognition – Swipe, tilt, and lift detection
* Multi-Device Control – LED dimming, fan ON/OFF, curtain open/close
* Noise Filtering – Deadzone + averaging for stable readings
* LCD Feedback – Real-time status display
* Calibration – Automatic sensor calibration

## Tinkercad Diagram for Wiring Assistance
In working.

## Hardware Components
* Arduino Uno
* MPU6050 (Accelerometer + Gyroscope)
* Servo Motors (x2)
* 16x2 I2C LCD
* LEDs (x2)
* DC Fan
* Relay Module
* Power Supplies (x2)
* 9V batteries (x2)
* Resistors & Jumper Wires

## Installation
1. Clone the repository
2. Upload the code to Arduino
3. In your Arduino IDE, go to Library Manager and download:
   * LiquidCrystal I2C by Frank de Brabander
4. Clone and upload all the repositories provided in the code
5. Connect hardware

## Calibration Guide
Before testing:
* Keep the MPU6050 sensor steady on a flat surface
* Wait a few seconds while the LCD displays "Calibrating... Keep hand still!"
* Do not move until the screen shows "Ready for gestures!"

NOTE: Automatic calibration is still under working. For best results:
* Connect the MPU6050 to the system using a HC-05 Bluetooth module instead of wires.
* Recalibrate if the device is moved to a new location.
