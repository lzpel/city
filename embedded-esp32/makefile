create:
	cargo install cargo-espflash --locked
	cargo install espup --locked
	espup install
generate:
	rustup override set esp
test:
	ls out 2>&1 >/dev/null || git clone https://github.com/esp-rs/esp-idf-hal out
	cd out && cargo espflash flash --target xtensa-esp32-espidf --example ledc_simple --release --monitor
clean:
	rm -rf out
