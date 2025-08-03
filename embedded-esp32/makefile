create:
	cargo install espup --locked
	espup install
generate:
	rustup override set esp
test:
	git clone https://github.com/esp-rs/esp-idf-hal out
	cd out && MCU=esp32c3 cargo espflash flash --target riscv32imc-esp-espidf --example ledc_simple --monitor