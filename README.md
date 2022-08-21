# Personal VPN
## Shadowsocks+V2Ray-plugin

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/kanjvt/shadowsocks-heroku/tree/main)

## 1. Verifikasi

https://test.herokuapp.com jika tampil 403 artinya sudah sukses deploy

## 2. Konfigurasi

QR code address: https://test.herokuapp.com/qr/vpn.png

pake shadowshock untuk scan qr code (rekomen)

**atau**

konfigurasi file -> Address: https://test.herokuapp.com/qr/

copy semua ke shadowshock

**atau**

Manual konfigurasi :

```sh
Server: test.herokuapp.com
Port: 443
Password: pass yg tadi deploy
Encry Method: chacha20-ietf-poly1305 (or other methods you fill in)
Plugin: v2ray
Plugin Transport mode: websocket-tls
Hostname: sama dgn server
Path: "/" + value of V2_Path in app Config Vars
```

tools untuk android :

[shadowsocks](https://github.com/shadowsocks/shadowsocks-android/releases/latest/download/shadowsocks--universal-5.1.9.apk)

[v2ray-plugin](https://github.com/shadowsocks/v2ray-plugin-android/releases/latest/download/v2ray-arm64-v8a-1.3.1.apk)

windows:

<https://github.com/shadowsocks/shadowsocks-windows/wiki/Shadowsocks-Windows-%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E>
