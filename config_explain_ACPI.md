
## ACPI

SSDT needed:

* ***SSDT-DDA.aml*** Fixing RMDA
* ***SSDT-NUC8-BC.aml*** NUC8 Bean Canyon model specific SSDT
* ***SSDT-TYPC-NUC8-BC.aml*** To manage NUC8 USBc
* ***SSDT-UIAC.aml*** To restrict USB ports

---
#### Patches :
* ***change _OSI to XOSI***
* ***change H_EC to EC***
* ***change GFX0 to IGPU***
* ***change HECI to IMEI***
* ***change SAT0 to SATA*** 
* ***change _DSM to XDSM***
* ***rename _RMV to XRMV***
* ***Fix NUC BIOS DSDT Device(RTC)***
