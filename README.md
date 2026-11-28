# Taeyoung Oh

I’m an Electronic Engineering senior at Tech University of Korea. I build and test embedded control systems that connect software, sensors, and actuators. My work spans autonomous vehicle controls, robot integration, vehicle electrical diagnostics, and STM32 firmware.

## Selected engineering work

### Autonomous vehicle control · Team NSSUR project lead

[Project repository and source download](https://github.com/oty-auto/nssur-autonomous-vehicle)

- Led five electrical and software contributors. Integrated camera, LiDAR, GNSS, and IMU data in ROS 2, and connected the C++ control software to STM32F439 steering, braking, and drive control over CAN. Designed the controller interface PCB, laid out the board, and tested it after fabrication.
- Replayed K-City sensor recordings to reproduce intermittent path loss, then revised how the controller retained and connected path updates. Added a guard against initial steering in the opposite direction and confirmed the corrected initial steering behavior at the wheels on the vehicle.
- Tuned Pure Pursuit using recorded data and tested the vehicle at K-City. Pretests covered straight driving, intersection turns, restart after a three-second stop, and straight passage through a signalized intersection without manual intervention.

### Go2 control integration · SkyAutoNet internship

- Diagnosed a DDS runtime conflict between ROS 2 Foxy and the C++ Unitree SDK. Restored command execution by separating ROS 2 command reception and SDK-based robot control into two processes connected over local UDP.
- Tested forward, reverse, rotation, and stop on a physical Go2. Interrupted incoming commands and compared logs with observed behavior to check a one-second timeout and a three-second watchdog stop. Troubleshot a RealSense D435i video stream and verified 720p at 30 fps on the monitoring interface.

### Formula Student electrical systems · Team NSSUR

- Redesigned and built two engine wiring harnesses, an installed harness and a spare. Traced an engine no-start condition to intermittent and open connections using continuity measurements and repaired the affected joints.
- Integrated CAN and programmed an STM32H747I-DISCO dashboard to display engine RPM, coolant temperature, and gear. Used an oscilloscope to inspect RPM and wheel-speed sensor signals.

### Automatic sun visor · Graduation project lead

- Implemented STM32F746ZG firmware that received a teammate’s vision output over UART and controlled two stepper motors. Designed the control circuitry, wired the hardware, and helped fabricate the mechanism.
- Used accumulated step counts to limit travel and return to the starting position. Verified deployment, lateral movement, stopping, travel limits, and return on the physical prototype.

## Tools and platforms

- **Software and control** · C, C++, Python, STM32CubeIDE, ROS 2, rosbag, RViz2, CARLA
- **Interfaces and hardware** · STM32, CAN, UART, UDP, KiCad, oscilloscope, multimeter
- **Additional training** · AURIX TC275 peripherals, CAN FD, CANoe, CAPL

## Conference work

- First author · *Design and Implementation of a Control System for a Self-Built Autonomous Vehicle for Lane and Intersection Driving* · 2026 KSAE Fall Conference and Exhibition
- First author · *Vehicle Automatic Sun Visor System Based on Driver Facial Shadow Recognition* · 2026 KICS Fall Conference
