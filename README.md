# Surveillance-Robot
This engineering project focuses on creating a surveillance robot with IR remote control and basic autonomous navigation. Using an ARM M4F microcontroller, it incorporates PIR, ultrasonic, and IR sensors for motion detection, obstacle avoidance, and command processing. A DRV8833 motor driver powers the robot's movement, supported by a safe 4xAA NiMH battery system.

<p align="center">
  <img src="Robot Front.jpg" alt="Robot Front" style="width: 500px;">
</p>
<p align="center">
  <b>Figure 1:</b> Image of the Product
  
## 💡 Key Features
<p align="center">
  <img src="Robot Travel.jpg" alt="Robot Front" style="width: 500px;">
</p>
<p align="center">
<b>Figure 2:</b> Robot on Autonmous Navigation

- **Remote Control:** Operates using an IR remote control with NEC protocol decoding.
- **Autonomous Navigation:** Uses ultrasonic sensors to detect and avoid obstacles.
- **Motion Detection:** PIR sensor detects heat sources and simulates alerts using on-board LEDs.
- **Odometry Feedback:** Optical interrupters provide wheel rotation data for tracking movement.
- **Compact Power Supply:** Powered by a 4xAA NiMH battery pack, ensuring safe voltage levels for all components.
- **Motor Control:** A DRV8833 dual H-bridge driver controls two DC motors for smooth operation.
- **Error Simulation:** On-board LEDs simulate error signals when motion is detected.
- **Modular Design:** 3D-printed components for the base, wheels, and sensor mounts provide easy assembly and customization.
- **Serial Communication:** A UART interface enables monitoring and debugging via a virtual COM port.

## 🛠 Hardware Components
  <p align="center">
  <img src="Robot Circuit Layout.jpeg" alt="Feeder Top" style="width: 500px;">
</p>
<p align="center">
  <b>Figure 2:</b> Circuit Layout

  |                         |
  | ------------------------|
  | - TM4C123GXL Board  |
  | - Dual H-bridge motor driver |
  | - DC Gearhead Motors x2 (Left Wheel & Right Wheel) |
  | - Passive Infrared(PIR) Sensor      |
  | - Ultrasonic sensor |
  | - IR Demodulator         |
  | - IR Led        x2 (Left Wheel & Right Wheel    |
  | - IR Phototransistor x2 (Left Wheel & Right Wheel |
  | - IR Remote Control |
  | - Passive Components |


## 🎛️ Capabilities

With UART communication, the robot can execute a 360-degree turn by independently controlling the motors to rotate the 3D-printed wheels in opposite directions, leveraging their lightweight design and enhanced grip provided by nitrile O-rings for precise and stable movement.

  <p align="center">
  <img src="Robot Angle Calculation.jpeg" alt="Feeder Top" style="width: 500px;">
</p>
<p align="center">
  <b>Figure 3:</b> This figure shows the process used for calculating the robot's angle and direction 
  
### Motor Control for Directional Movement:

- The dual H-bridge motor driver (DRV8833) enables independent control of two DC motors. By varying the PWM signals to the motors, the robot can move forward, backward, and make left or right turns.

### Odometry for Direction Tracking:
- The optical interrupters provide feedback on wheel rotation, which can be used to calculate the direction and distance traveled, allowing the robot to track its path.




  
