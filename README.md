# ESP32 binary merger

This script has been made to merge all bin file from ESP32 build, but can be used for other MCU type.

# Example

Merging 4 binaries : 

```
$ python merge_bin_esp.py --output_name app_output.bin --bin_path bootloader.bin app.bin partition-table.bin ota_data_initial.bin --bin_address 0x1000 0x10000 0x8000 0xd000
Add bootloader.bin from 0x1000 to 0x70f0 (0x60f0)
Add partition-table.bin from 0x8000 to 0x8c00 (0xc00)
Add ota_data_initial.bin from 0xd000 to 0xf000 (0x2000)
Add app.bin from 0x10000 to 0x155d80 (0x145d80)
app_output.bin generated with success !
```

