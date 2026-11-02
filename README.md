# Lenovo TB-X606V Dump Device
A quick guide on to Root your Lenovo Android Tablet for **`TB-X606V`** model using Magisk 🐣

> `Device warranty is void.` <br>
 `I'm not responsible for your device bricked. .` <br>
 `Your solely responsible for your own damage.` <br>
 
>

Requirements
---------------
- USB cable of your Tablet which you want to **`Root`**.
- Laptop is a must for rooting your device.

> `I assume that you have a laptop with NO broken ports / issues with USB.` <br>
`Not to proceed if you have a Bad USB cable which is damaged.` <br> 
`Your device will be bricked and cannot be recovered.` <br>

Prerequisites
-------------
- You need to install `adb` and `fastboot` which is known as `platform-tools`.
- Magisk App installed.
- Enable Developer Options.
- Turn on USB debugging and OEM bootloader unlock.
- Download the images from [releases](https://github.com/SurendraS26/tb-x606v-root/releases).

Installation Guide
------------------

**1. Reboot the device to fastboot mode**  

```bash
> adb reboot bootloader
```

**2. Check for fastboot devices**

```bash
> fastboot devices
```

**3. Unlock the flashing mode using `fastboot`**

```bash
> fastboot flashing unlock
```
  
**4. Push the `boot.img` file to device**

```bash
> adb push boot.img /sdcard/Download/
```
  
**5. Patch the `boot.img` with Magisk app**
- Open Magisk app. <br>
- Click **Install**. <br>
- Select and patch a file. <br>
- Choose the `boot.img`. <br>
- You will have the patched image in Downloads folder named as `magisk_patched-xyz.img`. <br>


**6. Pull the patched image from the device `magisk_patched-xyz.img`**

```bash
> adb pull /sdcard/Download/magisk_patched-xyz.img
```

**7. Reboot the device back to fastboot mode**

```bash
> adb reboot bootloader
```

**8. Flash the patched boot.img to device**

```bash
> fastboot flash boot magisk_patched-xyz.img
```

**9. Reboot your device**

```bash
> fastboot reboot
```

After the reboot, and you'll see your device is rooted 😊
> `Just be careful cause rooted device are even more riskier to maintain.`

