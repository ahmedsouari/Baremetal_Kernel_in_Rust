# Baremetal_Kernel_in_Rust

This project demonstrates how to create a minimal kernel in Rust for Raspberry Pi 3 Model B, which blinks an LED in a bare-metal environment.

Requirements :

    Raspberry Pi 3 Model B

    LED,breadboard,520 ohm resistor

    Rust toolchain ( add the armv7a-none-eabi by taping this command :

      $ rustup target add armv7a-none-eabi

Getting Started :

Cloning the Repository :

	$ git clone https://github.com/ahmedsouari/Baremetal_Kernel_in_Rust

Getting into the Rust Project

	$ cd Baremetal_Kernel_in_Rust/blinking

Building the Kernel

	$ make 

Deploying to Raspberry Pi :

Transfer the compiled kernel7.img to your Raspberry Pi's SD card. Don't forget to add Raspberry firmware files to the SD Card (bootcode.bin , start.elf , fixup.dat) Add to these files a config.txt file containing the following line " arm_64bit=0 " to insist that the enviremont should be 32 bit

Enjoy the blinking :

Insert the SD card into your Raspberry Pi and power it on. The LED connected to GPIO pin 21 should start blinking.

A detailed explanation of the source code is coming soon !
