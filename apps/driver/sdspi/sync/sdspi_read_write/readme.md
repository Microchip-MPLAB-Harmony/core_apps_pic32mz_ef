---
parent: Harmony 3 driver and system service application examples for PIC32MZ EF family
title: SDSPI driver synchronous - SDSPI Read Write 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# SDSPI driver synchronous - SDSPI Read Write

This example application shows how to use the SDSPI driver in synchronous mode to perform block operations on the SD Card Media

## Description

- The synchronous mode of the SDSPI driver is configured to use DMA and performs blocking read and write operations

- This example uses the SDSPI driver in synchronous mode in an RTOS environment

- A separate RTOS thread is created by the MHC to run the SDSPI task routine. This task routine checks for the SD-Card attach/detach status and initializes the SD-Card making it ready for the application to submit read and write requests

- This application writes 10KB (10240 bytes) of data starting at the SD Card memory location 0x2000
- The application then reads and verifies the written data

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/sdspi/sync/sdspi_read_write/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| pic32mz_ef_sk_freertos.X | MPLABX project for [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| pic32mz_ef_sk_freertos.X | [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) |
|||

### Setting up [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007)

- To run the demo, the following additional hardware are required:
    - [Multimedia Expansion Board II](https://www.microchip.com/Developmenttools/ProductDetails/DM320005-2)
    - One micro-sd card

- Mount the [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) on to the [Multimedia Expansion Board II](https://www.microchip.com/Developmenttools/ProductDetails/DM320005-2)

- Insert the micro-SD Card in the micro-SD Card slot of the [Multimedia Expansion Board II](https://www.microchip.com/Developmenttools/ProductDetails/DM320005-2)

- Connect the Debug USB port on the board to the computer using a mini USB cable

## Running the Application

1. Build and program the application using its IDE
2. The LED is turned ON when the read data from the SD card matches with the written data

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) | LED1 |
|||
