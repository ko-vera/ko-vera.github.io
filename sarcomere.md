## Sarcomere Dynamics
Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home) (Jan 2026 - Aug 2026)

- Designed the circuit, specified components, and laid out a PCB for a power management board (BMS) converting an 11.1V input to 5V (Raspberry Pi) and 24V (grippers in the Sarcomere product line) for a portable demo unit; sized trace widths and via counts per IPC-2221 to meet 7A/3A output requirements, and optimized MOSFET placement to minimize switching loop inductance.
- Led refactoring of communication architecture in C/C++ for the Artus Lite robotic hand, including MODBUS slave implementation (command parsing, register mapping, response frame generation) to improve modularity and standardize with the broader robotic gripper codebase.
- Reworked the Python user API’s MODBUS master implementation to align with the refactored slave-side protocol and standardize communication across the gripper product line, including support for communication across UART, RS485, and Wi-Fi TCP to ensure reliable end-to-end communication.
- Used FreeRTOS to manage inter-task communication across three concurrent tasks, including system scheduling and SPI mutex locking/blocking for resource management.
- Built a state machine to manage SD card read/write operations for storing actuator calibration data (end stops & range of motion) as well as last known grasp position, enabling the hand to restore to a known state after power loss.
- Developed functionality for firmware to be pushed through the user API, removing the need to physically connect individual actuator boards for field updates.
- Performed system-level debugging and integration between legacy and refactored architectures, ensuring compatibility and reliable operation.
- Tested and tuned control for robotic fingers and wrist through PID tuning and Python scripting; board bring up; diagnosed firmware, software, and hardware issues using data trend analysis, mechanical failure mode analysis, and oscilloscope inspection of CANBUS signals.
- Implemented impedance control so the wrist and fingers yield to external interference and return to position – critical for safe human-robot interaction.
  
<img src="/assets/hand-display-11.png" width="350">
