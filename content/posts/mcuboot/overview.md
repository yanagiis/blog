---
title: "MCUboot Overview"
date: 2021-10-11T19:10:49+08:00
draft: true
---

## What is MCUboot?

`Secure bootloader for 32-bit microcontrollers.`

It is a library which can be integrated into your bootloader to perform firmware upgrade securely.
For now, it works with both the Apache Mynewt and Zephyr operating system.

## Code structure

* boot/bootutil: The bootutil library. perform most of bootloader features
* boot/boot_serial: support serial recovery mode
* boot/[zephyr,mbed,nuttx,espressif,...]: The boot applications.

## Design

References:
1. https://www.mcuboot.com/
2. https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/mcuboot/design.html
3. https://interrupt.memfault.com/blog/mcuboot-overview#what-is-mcuboot
4. https://github.com/mcu-tools/mcuboot
