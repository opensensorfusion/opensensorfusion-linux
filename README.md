# Open Sensor Fusion Linux

This repository tracks Linux host-side work for Open Sensor Fusion hardware.

The upstream path is the Linux kernel mailing list. This repository is a
project mirror and documentation location for RFC work; it is not a replacement
for upstream kernel review.

## Current RFC Scope

The current driver work targets OSF GREEN and the OSF0 UART frame stream.

Host path tested during RFC preparation:

STM32F405 OSF0 UART stream -> Raspberry Pi 4 serdev -> Linux IIO raw and
buffer reads.

Observed IIO device names:

- `osf-accel`
- `osf-gyro`
- `osf-magn`
- `osf-temp`

## Not In Current Upstream RFC

- private ioctl
- broad custom sysfs ABI
- calibration command ABI
- USB transport
- Web Serial JSON demo output
- yaw debug frames
- fusion/AHRS/Kalman output
- production timestamp correlation claim

## Related Repositories

- https://github.com/opensensorfusion/opensensorfusion-hardware
- https://github.com/opensensorfusion/opensensorfusion-firmware

## License

Linux driver code is intended to use `GPL-2.0-only`. See `LICENSES/`.
