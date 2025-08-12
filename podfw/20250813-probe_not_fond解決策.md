smith@DESKTOP-S0G7BVU MINGW64 ~/Downloads/city/podfw (main)
$ RUST_LOG="debug" probe-rs run --chip nRF52840_xxAA --probe "1366:1015" "target/thumbv7em-none-eabihf/release/blinky"
DEBUG probe_rs::cmd::run: No embedded-test in ELF file. Running as normal
DEBUG list_cmsisdap_devices: probe_rs::probe::cmsisdap::tools: Searching for CMSIS-DAP probes using nusb
DEBUG list_cmsisdap_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_cmsisdap_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_cmsisdap_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_cmsisdap_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_cmsisdap_devices: probe_rs::probe::cmsisdap::tools: Found 0 CMSIS-DAP probes using nusb, searching HID
DEBUG list_cmsisdap_devices: probe_rs::probe::cmsisdap::tools: Found 0 CMSIS-DAP probes total
DEBUG list_ftdi_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_ftdi_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_ftdi_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_ftdi_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_stlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_stlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_stlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_stlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_jlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_jlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_jlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_jlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_espjtag_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_espjtag_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_espjtag_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_espjtag_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_wlink_devices: probe_rs::probe::wlink: Searching for WCH-Link(RV) probes
DEBUG list_wlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG list_wlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG list_wlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG list_wlink_devices: nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG list_wlink_devices: probe_rs::probe::wlink: Found 0 WCH-Link probes total
DEBUG postcard_rpc::host_client::util: Handled message via map
DEBUG probe_rs::config::registry: Searching registry for chip with name nRF52840_xxAA
DEBUG probe_rs::config::registry: Exact match for chip name: nRF52840_xxAA
 INFO probe_rs::config::target: Using sequence Arm(Nrf52)
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG probe_rs::probe::cmsisdap::tools: Attempting to open 1366:1015 in CMSIS-DAP v1 mode
DEBUG probe_rs::probe::stlink: Opening ST-Link: DebugProbeSelector { vendor_id: 4966, product_id: 4117, serial_number: Some("000682518146") }
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG nusb::platform::windows_winusb::device: Creating device for "USB\\VID_1366&PID_1015\\000682518146"
DEBUG probe_rs::probe::jlink: scanning 4 interfaces
DEBUG probe_rs::probe::jlink: J-Link interface is #2
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1366&PID_1015\\000682518146"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_1C4F&PID_0027\\8&18D650E6&0&1"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_0C45&PID_7B36\\8&18D650E6&0&4"
DEBUG nusb::platform::windows_winusb::enumeration: Probing device "USB\\VID_8087&PID_0032\\6&3A276F1F&0&5"
DEBUG postcard_rpc::host_client::util: Handled message via map
Error: Probe not found

<img width="575" height="254" alt="Image" src="https://github.com/user-attachments/assets/6a396903-8892-4595-9ec3-6740f55e6024" />
https://probe.rs/docs/getting-started/probe-setup/

>Windows: WinUSB drivers
>Some of the probe implementations are implemented using nusb which uses the WinUSB drivers on Windows. For these devices you will need to download Zadig and select WinUSB as the driver for your probe. This will uninstall any official drivers, which means that the official tools will most likely not work anymore after this