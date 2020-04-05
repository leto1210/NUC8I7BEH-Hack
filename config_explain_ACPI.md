
## ACPI

SSDT needed:
* ***SSDT-NUC8-BC.aml*** NUC8 Bean Canyon model specific SSDT
* ***SSDT-TYPC-NUC8-BC.aml*** To manage NUC8 USBc
* ***SSDT-UIAC.aml*** To restrict USB ports

---
#### Patches :
* ***change EC0 to EC*** To enable USB power management
* ***RTC fix***
* ***change PEPG to GFX0***
* ***change GFX0 to IGPU***
* ***change XHCI to XHC*** Helps avoid a conflict with built-in USB injectors
* ***change SAT0 to SATA*** Need for correct mapping of my SATA drive
* ***change HDAS to HDEF***
