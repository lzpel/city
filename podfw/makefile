export RE_PATH=s/,\s+path\s*=\s*["'][^"']+["']//
export RE_HF=s/eabi(["'])/eabihf\1/;s/nRF52840_xxAA/nRF52832_xxAA/
export RE_MEM=s/1024K/512K/;s/256K/64K/
create:
	cargo install probe-rs-tools --locked
	probe-rs complete install
create-template:
	ls out || git clone --recursive https://github.com/embassy-rs/embassy.git out
	cp -r out/examples/nrf52840/. .
	perl -i -pe $${RE_PATH} Cargo.toml
	perl -i -pe $${RE_HF} .cargo/config.toml
	perl -i -pe $${RE_MEM} memory.x
run:
	cargo run --release --bin embassy-nrf52840-examples