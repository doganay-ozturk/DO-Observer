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
  - **Electronic Control Unit**:[STM32F4-Discovery Board](https://www.mouser.fr/ProductDetail/STMicroelectronics/STM32F407G-DISC1?qs=mKNKSX85ZJejxc9JOGT45A%3D%3D&srsltid=AfmBOoragK4ADnajOwfYKngf64bH2ytlkqvQkB8ivC5R5yLmAn2ZQwac)
  - **Ethernet**: [W5500 Module](https://www.amazon.fr/Hailege-Ethernet-Network-Support-Microcontroller/dp/B0CJY22SWF?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&psc=1&smid=A1A7E5ILEFA1R3)
  - **Cellular & GNSS**: [Waveshare SIM7070G HAT](https://www.waveshare.com/sim7070g-cat-m-nb-iot-gprs-hat.htm)
  - **SIM Card**: [Things Mobile IOT SIM](https://www.thingsmobile.com)
  - **Display**: [0.96" I2C OLED](https://www.thingsmobile.com)
  - **Obstacle Detection**: [SLAMTECH RPLIDAR C1](https://bucket-download.slamtec.com/2d4664be9f9f5c748f3b608f2cf1862962b168eb/SLAMTEC_rplidar_datasheet_C1_v1.1_en.pdf)
## Software & Development Environment
  - **Operating System**: [FreeRTOS](https://www.freertos.org/)
  - **HAL**: [STM32 HAL Libray](https://github.com/STMicroelectronics/stm32f4xx-hal-driver)
  - **Development Tools**
    - Arch Linux ([Host OS](https://archlinux.org/))
    - [Neovim](https://neovim.io/): A modern, extensible Vim-based text editor
    - [Cmake](https://cmake.org/) (Build System)
    - ARM GCC ([Compiler](https://developer.arm.com/downloads/-/gnu-rm))
    - [OPENOCD](https://openocd.org/) (flashing / debugging via SWD)
    - [Docker](https://www.docker.com/): Used to containerize the full development environment, ensuring consistency, portability, and easy onboarding for all contributors.


