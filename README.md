# OpenWrt-NanoPi-R5s-Firmware
OpenWrt aarch64 firmware for Firendly NanoPi R5s,  based on [Lean's LEDE source](https://github.com/coolsnowwolf/lede).

Added package:
- OpenClash
- subconverter 
- ArgonTheme
- ArgonConfig

Enabled package
- Docker Man
- Docker compose
- qBittorrent
- Samba
- Aria2
- Zerotier
- Netdata 
- QoS
- UUGameBooster

Added Kernel Support
- kmod-usb-acm
- kmod-ip6tables


## Notes

### OpenClash & subconverter

It can convert subscription URLs locally, see https://github.com/tindy2013/subconverter. Just use `http://127.0.0.1:25500/sub?` as the converter address.

Please note that the subscription URL must be processed by urlencode before converting, see the README of subconverter.

For example:

```bash
sudo apt install urlencode
urlencode <https://your.subscription.url>
```

## kmod-usb-acm & kmod-ip6tables

These can support OpenThread Board Router (OTBR) container, make your R5s a Thread Board Router. You need a RCP (Radio Co-processor), like a nRF52840 Dongle with RCP firmware.

<img src="https://raw.githubusercontent.com/Jayant-Tang/OpenWrt-NanoPi-R5s-Firmware/master/picture/BoardRouter.jpg" alt="Board Router" style="zoom: 25%;" />

>  For more information about OpenThread, see:
>
> - https://openthread.io/ 
> - https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/protocols/thread/tools.html#thread-tools



