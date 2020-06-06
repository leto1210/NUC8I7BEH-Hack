# SSDT (USB)

In this configuration, we disabled one internal port HS06.

* Open About This Mac > System Report > Hardware > USB
* Take note of the USB 3.1 Bus PCI Device ID (0xa36d)
* Open SSDT-UIAC-ALL.dsl in MaciASL
* Find the section which matches the above PCI Device ID, and remove all other sections
* The current SSDT-UIAC file is configured as follows:
    * HS01: USB 3.1 Front - ENABLED
    * HS02: USB 3.1 Front - ENABLED
    * HS03: USB 3.1 rear - ENABLED
    * HS04: USB 3.1 rear - ENABLED
    * HS05: USB 2.0 connector - ENABLED (Used for Broadcom bluetooth PCI adapter)
    * HS06: DISABLED
    * SS01: ENABLED
    * SS02: ENABLED
    * SS03: ENABLED
    * SS04: ENABLED
* Compile as `SSDT-UIAC.aml` file to `EFI/ACPI/`
* Disable USB port limit patch in OpenCore

```
[File Example](./SSDT/SSDT-UIAC.dsl)
```


> If you prefer, Hackintool can generate the right files for you ;-)
