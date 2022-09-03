## Update

cd /home/pi/klipper
make menuconfig

- STM32
- STM32F446
- No Bootloader
- 12mz Crystal
- USB PA11/PA12

make

boot in dfu  (power off board, turn on dfu, power on)

dfu-util -R -a 0 -s 0x08000000:leave -D out/firmware.bin

turn off dfu



## Cura settings
PRINT_START BED_TEMP={material_bed_temperature_layer_0} EXTRUDER_TEMP={material_print_temperature_layer_0} CHAMBER_TEMP={build_volume_temperature}  LAYER_HEIGHT=0.3

PRINT_END