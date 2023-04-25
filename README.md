# OpenWrt-NanoPi-R5s-Firmware
OpenWrt aarch64 firmware for Firendly NanoPi R5s,  based on [Lean's LEDE source](https://github.com/coolsnowwolf/lede).

Added package:
- OpenClash
- subconverter (http://127.0.0.1:25500/sub?)
- Docker Man
- Docker compose
- qBittorrent (localhost:8080)
- Samba
- Aria2
- Zerotier
- Netdata (localhost:19999)
- QoS
- UUGameBooster
- ArgonTheme & ArgonConfig

## Notes

### OpenClash & subconverter

It can convert subscriptions locally, see https://github.com/tindy2013/subconverter. Just use `http://127.0.0.1:25500/sub?` as converter address.

Please note that the subscription URL must be processed by urlencode, see the README of subconverter.

```bash
sudo apt install urlencode
urlencode <https://your_subscription_url>
```
