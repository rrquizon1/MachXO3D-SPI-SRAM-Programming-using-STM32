This is an SSPI programming example using STM32F411 

This example uses STM32F411 using STM32 HAL SPI Drivers and GPIO control for CS similar to previous Raspberry Pi 5 SPI example.

The instructions used in this program follows the guideline of FPGA-TN-02069-1.7(MachXO3D Programming and Configuration User Guide)

MachXO3D's compressed bitstream is still within the Raspberry Pi's buffer limit, so we can send all the data in one call.

In this implementation you can modify the array in data.c with your own bitstream.
![image](https://github.com/user-attachments/assets/cacc6500-35df-4601-bd66-c9bf474d655c)

Compared to ice40 programming implementation using STM32F411, MAchXO3D SRAM programming needs a few more lines but still a lot more simple because of STM32 HAL drivers. See below for some functions I used to implement the programming flow:
![image](https://github.com/user-attachments/assets/581a0122-385d-48e4-8b3d-9d7e4146b01f)

Sample terminal run: 
![image](https://github.com/user-attachments/assets/8935675f-31a1-4256-baae-a6e06c28ffbe)





