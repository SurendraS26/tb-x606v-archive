# Lenovo TB-X606V Root Device
A quick guide on to Root your Lenovo Android Tablet for **`TB-X606V`** model using Magisk 👻


> **`My friend your device warranty is void.`** <br>
 **`I'm not responsible for your device being bricked.`** <br>
 **`Your solely responsible for your own damage.`**
>

Requirements
-------------
- USB cable of your Tablet which you want to **`Root`**.
- Laptop is a must for rooting your device.

> **`I assume that you have a laptop with NO broken ports / issues with USB.`** <br>
**`Not to proceed if you have a Bad USB cable which is damaged.`** <br> 
**`Your device will be bricked and cannot be recovered.`** <br>

Prerequisites
-------------
- You need to install `adb` and `fastboot` which is known as `platform-tools`.
- Magisk App installed.
- Enable Developer Options.
- Turn on USB debugging and OEM bootloader unlock.
> Note: Your almost there to root this device. 

Installation Guide
------------------
- Unlocking Bootloader

  - Reboot the device to fastboot mode
  
    ```bash
    > adb reboot bootloader
    ```
  - Check for fastboot devices

    ```bash
    > fastboot devices
    ```
  - Unlock the flashing mode using `fastboot`

    ```bash
    > fastboot flashing unlock
    ```
> Note: You need to confirm the unlock on your phone screen.


