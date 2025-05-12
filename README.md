# DO-Observer
DO-Observer is an autonomous terrain vehicle project. The STM32F4-Discovery board serves as the Electronic Control Unit (ECU), managing real-time control, sensor fusion, and communication for robust outdoor navigation and observation.
A docker image is provided to simplify setup and ensure a consistent build environment across all platforms. 

## Features 
- **Autonomous Navigation**
  > GNSS(GPS) for global positioning and SLAMTECH RPLIDAR C1 for real-time obstacle detection and avoidance.
- **Dynamic Observation**
  > Real-time sensor fusion and advanced control algorithms for adaptive, intelligent navigation.
- **Status Display**
  > 0.96" I2C OLED screen for system status and diagnostics. This could be changed with touch LED screen in the future.
- **Modular & Expandable**
  > Architecture supports additional sensors or features.

## Hardware Components
  - **Electronic Control Unit**: STM32F4-Discovery Board
  - **Ethernet**: W5500 Module
  - **Cellular & GNSS**: Waveshare SIM7070G HAT
  - **SIM Card**: Things Mobile IOT SIM
  - **Display**: 0.96" I2C OLED
  - **Obstacle Detection**: SLAMTECH RPLIDAR C1
## Software & Development Environment
  - **Operating System**: FreeRTOS
  - **HAL**: STM32 HAL Libray
  - **Development Tools**
    - Arch Linux ( Host OS)
    - Neovim: A modern, extensible Vim-based text editor
    - Cmake (Build System)
    - ARM GCC (Compiler)
    - OPENOCD (flashing / debugging via SWD)
    - Docker: Used to containerize the full development environment, ensuring consistency, portability, and easy onboarding for all contributors.


