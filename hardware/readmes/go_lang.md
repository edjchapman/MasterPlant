Sensor Software in Go Lang
==========================

### Environment Setup

1. Setup TinyGo
```shell
https://tinygo.org/getting-started/
```

2. Attach Arduino with USB and find the port number
```shell
ls /dev/* | grep modem/
# ls /dev/* | grep serial/ # If none found
```

3. Run test "blink" program to confirm its working
```shell
tinygo flash -target=arduino -port=[PORT] hardware/go_lang/blinky.go
# e.g.
# tinygo flash -target=arduino -port=/dev/tty.usbmodem142101 hardware/go_lang/blinky.go
```