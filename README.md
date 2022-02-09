## Setup

Set these enviroment variables via `export` or GitPod project variables.

| Name      | Description / Reasoning |
| ----------- | ----------- |
| `PLATFORMIO_GLOBALLIB_DIR` | The esphome docker image sets `/piolibs` as a envvar which isn't writable with Gitpod |
| `NETWORK_KEY` | Wifi network key / password |
| `SSID` | Wifi network name / SSID |
| `OTA_PASSWORD` | OTA password |


## Build firmware
1. `./wrapper.sh compile {yaml}`
1. Download `firmware.bin` from `.esphome/build/{esphome name}/.pioenvs/{esphome name}/firmware.bin`
1. OTA upload `firmware.bin`
