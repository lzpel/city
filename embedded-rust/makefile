create: create-install create-udevrules create-dialout
	@: complete
create-install:
	sudo apt install minicom libusb-1.0-0-dev libsdl2-dev libssl-dev
	cargo install cargo-generate
	@: PKG_CONFIG_PATH=/usr/local/lib/pkgconfig:/usr/lib/pkgconfig cargo install hf2-cli
	cargo install hf2-cli
	cargo install cargo-hf2
create-udevrules:
	bash -c "$${create}"
	sudo udevadm control --reload-rules
create-dialout:
	sudo adduser "$${USER}" dialout
define create
sudo install -D /dev/stdin /etc/udev/rules.d/99-seeed-boards.rules <<EOF
ATTRS{idVendor}=="2886", ENV{ID_MM_DEVICE_IGNORE}="1"
SUBSYSTEM="usb", ATTRS{idVendor}=="2886", MODE="0666"
SUBSYSTEM="tty", ATTRS{idVendor}=="2886", MODE="0666"
EOF
endef
export create
