build :	
	cargo rustc -- -C link-arg=--script=./linker.ld
	arm-none-eabi-objdump -D target/armv7a-none-eabi/debug/blinking | less
	arm-none-eabi-objcopy -O binary target/armv7a-none-eabi/debug/blinking kernel7.img 
	