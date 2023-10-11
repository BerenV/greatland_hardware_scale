# greatland_hardware_chopper
Documentation for CNC sliding scale attached to a pneumatic-hydraulic Roto hardware chopper with barcode scanning and keypad entry. 

The barcode scanner is in its default mode for everything (USB_HID). The USB receiver for it is wired directly to a Raspberry Pi Pico which acts as the host and sends keypresses over hardware UART serial at 115200 baud. The .uf2 file is included in case the Pico ever fails, but all I did is build the host_cdc_msc_hid example from the publicly available Pico examples at https://github.com/raspberrypi/pico-examples/tree/master/usb/host/host_cdc_msc_hid. I wasn't smart enough to change any of the code.
