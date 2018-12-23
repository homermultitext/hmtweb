---
title: "Notes on Setting BIOS for the HMT VM"
layout: page
---


- **Windows 8 and 8.1**:  see [this page with instructions for editing UEFI BIOS](http://acer.custhelp.com/app/answers/detail/a_id/27103/~/accessing-the-uefi-(bios)-setup-on-a-windows-8-%2F-8.1-system) (from Acer)
-  **Windows Vista**:  restart the computer and look in the upper-right corner of the screen; very briefly, instructions will flash by, telling which function-key to hold down to enter the BIOS settings.

The setting that needs to be enabled goes by the following names: `VT-x`, `Intel Virtualization Technology`, `Vanderpool Technology`.

## Known successes and failures

- HP Elitebook with Windows 8 works?
- A Dell Inspiron 1420 cannot run a Vagrant VM.

## Some Images of Particular Maker's Settings

- Lenovo ![lenovo](../imgs/lenovo_bios.jpg)
