---
parent: Harmony 3 driver and system service application examples for PIC32MZ EF family
title: Memory driver asynchronous - NVM SST26 Read Write  
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Memory driver asynchronous - NVM SST26 Read Write 

This example application shows how to use the Memory driver in asynchronous mode to perform block operations on the NVM and the SST26 media's.

## Description

### This application:

- Uses multi instances of the Memory driver to communicate with the NVM and the SST26 Flash memories in asynchronous mode of operation in Bare-Metal environment

- Performs block Erase/Write/Read operations on both the media's

- Consists of five tasks which are called through the SYS_Tasks() routine in Bare-Metal environment

    1. **DRV_MEMORY_0_Tasks():**
        - Manages the state machine of the Memory driver instance 0
    2. **DRV_MEMORY_1_Tasks():**
        - Manages the state machine of the Memory driver instance 1
    3. **APP_SST26_Tasks():**
        - Performs operations on the SST26 QSPI/SQI Flash memory
    4. **APP_NVM_Tasks():**
        - Performs operations on the NVM
    5. **APP_MONITOR_Tasks():**
        - Monitors the state of above two Tasks

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/memory/async/nvm_sst26_read_write/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| pic32mz_ef_sk.X | MPLABX project for [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| pic32mz_ef_sk.X | [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) |
|||

### Setting up [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007)

- Connect the Debug USB port on the board to the computer using a mini USB cable

## Running the Application

1. Build and program the application using its IDE
2. The LED is turned ON when the data read from each media matches with the data written in them

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [PIC32MZ Embedded Connectivity with FPU (EF) Starter Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/dm320007) | LED3 |
|||