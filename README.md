# T440p-Misc-BIOS-patches
Miscelanious BIOS patches for the T440p


Here is my new creation for fellow T440p users: some MISC bios patches. These patches assume you already have flashed the general thinkpad UEFI patches with advanced menu unlock and know how to use a SPI programmer.

The 1st patch unlocks SATA options (AHCI/IDE) useful if you wanna install windows XP or something, along with stuff like disabling the Fn key for waking from sleep, or disabling the internal battery, which as stupid as it is, works as intended.

2nd patch sets the default PROCHOT throttling value to 100degC, rather than the stock 92, the changes should take effect once you reset BIOS settings to defaults.

3rd patch just unhides CFG Lock option in advanced settings, useful for hackintosh users.

And the 4th patch enables spoofing of the touchpad ACPI ID to the one of T570. This allows you to install latest T570 precision touchpad drivers without any tweaking, inf modding etc. and is permanent. The only downside is that if you use the original T440p trackpad, the top trackpoint "buttons" don't work.

If you wish to omit a certain patch, open the patches.txt file and place # at the beginning of the line with the particular patch.

Usage: UEFIPatch.exe romname.rom patches.txt
