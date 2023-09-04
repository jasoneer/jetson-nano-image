<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()

</div>

# Feedback

I'm planning to actively work on this project again from September.

What would you like to have as tools and setup for the minimalist image ?

Let me know by opening an issue.

## Dependencies:
* Ubuntu host
* podman
* just
* jq
* qemu-user-static

## Instructions:

**Building image**
```
$ git clone https://github.com/pythops/jetson-nano-image
$ cd jetson-nano-image

$ just build-jetson-rootfs
$ just build-jetson-image jetson-nano 300
```

**Flashing to SD card**
```
$ sudo just flash-jetson-image <jetson image file> <sdcard device>
```

**Install NVIDIA libs (on board boot)**
```
$ sudo apt install -y cuda-toolkit-10-2 libcudnn8 libcudnn8-dev
```

## Spec:

**Ubuntu release**: 20.04 focal

**BSP**: 32.7.4

## Supported boards:

- [Jetson nano](https://developer.nvidia.com/embedded/jetson-nano-developer-kit)
- [Jetson nano 2GB](https://developer.nvidia.com/embedded/jetson-nano-2gb-developer-kit)

## Looking for professional support ?

If you need more advanced configuration or a custom setup, you can contact me on this address support@pythops.com

## License

Copyright Badr BADRI @pythops

2019-2022 MIT

2023-Present AGPLv3
