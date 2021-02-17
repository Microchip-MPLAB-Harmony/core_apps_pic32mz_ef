---
title: Harmony 3 driver and system service application examples for PIC32MZ EF family
nav_order: 1
has_children: true
has_toc: false
---
[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Harmony 3 driver and system service application examples for PIC32MZ EF family

MPLAB® Harmony 3 is an extension of the MPLAB® ecosystem for creating embedded firmware solutions for Microchip 32-bit SAM and PIC® microcontroller and microprocessor devices.  Refer to the following links for more information.

- [Microchip 32-bit MCUs](https://www.microchip.com/design-centers/32-bit)
- [Microchip 32-bit MPUs](https://www.microchip.com/design-centers/32-bit-mpus)
- [Microchip MPLAB X IDE](https://www.microchip.com/mplab/mplab-x-ide)
- [Microchip MPLAB® Harmony](https://www.microchip.com/mplab/mplab-harmony)
- [Microchip MPLAB® Harmony Pages](https://microchip-mplab-harmony.github.io/)

This repository contains the MPLAB® Harmony 3 driver and system service application examples for PIC32MZ EF family

- [Release Notes](release_notes.md)
- [MPLAB® Harmony License](mplab_harmony_license.md)

To clone or download these applications from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef) and then click **Clone** button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

## Contents Summary

| Folder     | Description                             |
| ---        | ---                                     |
| apps       | Contains driver and system service example applications |
| docs       | Contains documentation in html format for offline viewing (to be used only after cloning this repository onto a local machine). Use [github pages](https://microchip-mplab-harmony.github.io/core_apps_pic32mz_ef/) of this repository for viewing it online. |

## Code Examples

The following applications are provided to demonstrate the typical or interesting usage models of one or more peripheral libraries.

| Name | Description |
| ---- | ----------- |
| [Memory driver asynchronous - NVM SST26 Read Write ](apps/driver/memory/async/nvm_sst26_read_write/readme.md) | This example application shows how to use the Memory driver in asynchronous mode to perform block operations on the NVM and the SST26 media's |
| [Memory driver synchronous - NVM SST26 Read Write ](apps/driver/memory/sync/nvm_sst26_read_write/readme.md) | This example application shows how to use the Memory driver in synchronous mode to perform block operations on the NVM and the SST26 media's.  |
| [SDSPI driver synchronous - SDSPI Read Write](apps/driver/sdspi/sync/sdspi_read_write/readme.md) | This example application shows how to use the SDSPI driver in synchronous mode to perform block operations on the SD Card Media |
| [SPI Driver asynchronous - Self loopback multi client](apps/driver/spi/async/spi_self_loopback_multi_client/readme.md) | This example demonstrates how to use the SPI driver in asynchronous mode to achieve self-loop back between multiple clients |
| [SPI Driver synchronous - Self loopback multi client](apps/driver/spi/sync/spi_self_loopback_multi_client/readme.md) | This example demonstrates how to use the SPI driver in synchronous mode to achieve self-loop back between multiple clients in RTOS environment |
| [SQI Flash SST26 driver - SST26 SQI Read Write](apps/driver/sqi_flash/sst26/sst26_sqi_read_write/readme.md) | This example application shows how to use the SST26 driver to perform block operations on the On-Board SST26 Flash memory in Quad IO mode |
| [USART driver asynchronous - USART echo](apps/driver/usart/async/usart_echo/readme.md) | This example echoes the received characters over the console using the USART driver in asynchronous mode |
| [USART driver synchronous - USART echo](apps/driver/usart/sync/usart_echo/readme.md) | This example echoes the received characters over the console using the USART driver in synchronous mode |
| [FAT filesystem using NVM Media](apps/fs/nvm_fat/readme.md) | This application shows an example of implementing a FAT disk in the device internal Flash memory |
| [MPFS filesystem using NVM Media](apps/fs/nvm_mpfs/readme.md) | This application shows an example of implementing a MPFS disk in device Internal Flash memory |
| [FAT filesystem using NVM and SDSPI Media](apps/fs/nvm_sdspi_fat_multi_disk/readme.md) | This application shows an example of using the MPLAB Harmony File System to access files across multiple media (NVM, SDSPI) |
| [FAT filesystem using NVM and SST26 Media](apps/fs/nvm_sqi_fat/readme.md) | This application shows an example of using the MPLAB Harmony File System to access multiple files across multiple media (NVM, SQI FLASH) |
| [FAT filesystem using SDSPI Media](apps/fs/sdspi_fat/readme.md) | This application shows an example of using the MPLAB Harmony File System to access and modify the contents of a SD card using the SDSPI driver and the SPI PLIB |
| [FAT filesystem using SST26 Media](apps/fs/sqi_flash_fat/readme.md) | This application shows an example of using the MPLAB Harmony File System to access SQI based SST26 flash media |
| [FreeRTOS basic](apps/rtos/freertos/basic_freertos/readme.md) | This example application demonstrates context switching between four tasks of different priorites. Two tasks run periodically while the other two tasks are event driven |
| [FreeRTOS Task Notification](apps/rtos/freertos/task_notification_freertos/readme.md) | This example application is to illustrate the FreeRTOS Task Notification feature which is used as a light weight binary semaphore |
| [Console Debug System Service using UART](apps/system/console_debug/sys_console_debug_uart_read_write/readme.md) | This example application demonstrates the UART based console and debug system service |
| [Console Debug System Service using USB](apps/system/console_debug/sys_console_debug_usb_read_write/readme.md) | This example application demonstrates the USB based console and debug system service |
| [Time System Service multi-client](apps/system/time/sys_time_multiclient/readme.md) | This example application demonstrates the multi-client system timer functionality |

____

[![License](https://img.shields.io/badge/license-Harmony%20license-orange.svg)](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef/blob/master/mplab_harmony_license.md)
[![Latest release](https://img.shields.io/github/release/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg)](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef/releases/latest)
[![Latest release date](https://img.shields.io/github/release-date/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg)](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef/releases/latest)
[![Commit activity](https://img.shields.io/github/commit-activity/y/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg)](https://github.com/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef/graphs/commit-activity)
[![Contributors](https://img.shields.io/github/contributors-anon/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg)]()

____

[![Follow us on Youtube](https://img.shields.io/badge/Youtube-Follow%20us%20on%20Youtube-red.svg)](https://www.youtube.com/user/MicrochipTechnology)
[![Follow us on LinkedIn](https://img.shields.io/badge/LinkedIn-Follow%20us%20on%20LinkedIn-blue.svg)](https://www.linkedin.com/company/microchip-technology)
[![Follow us on Facebook](https://img.shields.io/badge/Facebook-Follow%20us%20on%20Facebook-blue.svg)](https://www.facebook.com/microchiptechnology/)
[![Follow us on Twitter](https://img.shields.io/twitter/follow/MicrochipTech.svg?style=social)](https://twitter.com/MicrochipTech)

[![](https://img.shields.io/github/stars/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg?style=social)]()
[![](https://img.shields.io/github/watchers/Microchip-MPLAB-Harmony/core_apps_pic32mz_ef.svg?style=social)]()