# Free_RTOS
This project demonstrates the implementation of a Real-Time Operating System (RTOS) on the STM32F446RE development board. Using FreeRTOS, the project manages multiple tasks concurrently, ensuring deterministic and real-time performance for embedded applications.
How to Run This Project

# Follow these steps to easily set up and run the FreeRTOS project on your STM32F446RE development board:

1. Requirements
Hardware: STM32F446RE Nucleo or Discovery board, USB cable, and a PC.
Software:
STM32CubeIDE (Official IDE for STM32)
STM32CubeMX (Optional, for generating initialization code)
FreeRTOS (already included in STM32CubeIDE)
2. Open the Project
Download or clone the project repository to your PC.
Open STM32CubeIDE.
Go to File → Open Projects from File System.
Browse to the project folder and import it.
3. Configure the Board (if needed)
Ensure that the project is set for STM32F446RE in the project settings.
Verify that the clock configuration and peripherals (like UART, GPIO, or timers) match your hardware setup.
4. Build the Project
Click the Build button (hammer icon) in STM32CubeIDE.
Wait for the build to complete. Make sure there are no errors.
5. Flash the Firmware
Connect your STM32F446RE board to your PC via USB.
Click the Run button (green play icon) in STM32CubeIDE.
The IDE will program the board and start running the RTOS tasks.
6. Monitor Output (Optional)
If the project uses UART for debugging, open a serial terminal (e.g., PuTTY, Tera Term) with the following settings:
Baud rate: 115200 (or as configured)
Data bits: 8
Stop bits: 1
No parity
You should see real-time logs or task execution messages.
7. Customize or Add Tasks
Open the freertos.c or task source files.
Add or modify tasks using xTaskCreate() function.
Rebuild and flash to test your changes.
