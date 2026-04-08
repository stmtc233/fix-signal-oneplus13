# fix-signal-oneplus13

Fix signal for OnePlus 13 CN on OxygenOS 16.

[Download](https://github.com/stmtc233/fix-signal-oneplus13/releases)

> [!WARNING]
> **PSA: Anti-Rollback Protection**
>
> OnePlus has implemented anti-rollback protection starting with firmware version **16.0.3.50x**.
>
> If you are on **16.0.3.50x or higher**, **DO NOT downgrade** to any earlier version:
> * This will cause a **HARD BRICK**.
> * **Leaked EDL tools will not work.** Anti-rollback is specifically designed to block them.
> * Only official/authorized EDL access can fix this state.
>
> Please be careful when flashing any ROMs.
>
> ~~Never Settle.~~ **Sometimes Settle.**

## Tutorial

### How to fix signal

Download and install this module in Magisk (or other root manager).

### How to relock bootloader

**Please don't.**

Your device will **brick** if you relock the bootloader with any modifications to the system partition in **any** slot (e.g., root, custom kernel, etc.).

> [!CAUTION]
> **This module is for rooted users. You **MUST** keep your bootloader unlocked. Do NOT lock the bootloader.** <br>
> 
> To relock the bootloader, you **MUST** remove root and restore the device to stock state.<br>
> **Relocking the bootloader is a dangerous operation.** Do not relock your bootloader unless you fully understand what you are doing.<br>
> On OnePlus 13, you cannot access fastboot again via key combination if the bootloader is locked.<br>
> If you lock your bootloader while rooted or modified, your phone will hard brick and cannot be recovered by yourself.
>
> If **any** of the following are not met, relocking the bootloader **will brick your device**:
>
> * **Every system partition in BOTH slots must be 100% stock and unmodified.**
>   * To ensure this, after restoring the latest version of stock OS on your device, download the full OTA ROM (.zip) for that OS version and local install it TWICE: local install, then reboot, then local install it AGAIN.
>   * Be very careful when rolling back to an older OS version. If your device has upgraded to an OS version with anti-rollback, downgrading to any earlier version will brick it. **Please read [the warning](#fix-signal-oneplus13) above.**
> * **Google account must be removed.**
>   * On older ColorOS / OxygenOS versions, due to a critical bug, FRP (Factory Reset Protection, a.k.a. activation lock) prevents completing the initial setup, effectively bricking it.

----

## Thanks to

- [@koaaN](https://xdaforums.com/m/koaan.3433581/)

- [@docnok63](https://xdaforums.com/m/docnok63.4967345/)

- [rapperskull](https://github.com/rapperskull)

## Maintainer Workflow

Run the `Update Module From Firmware Archive` workflow manually from the Actions tab to pull the latest `PJZ110` `image-firmware` package, refresh `oplusstanvbk.img`, update module metadata, and publish a new module release.





