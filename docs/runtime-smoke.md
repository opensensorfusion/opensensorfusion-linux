# Runtime Smoke

Raspberry Pi 4 smoke testing was used during RFC preparation.

Observed path:

STM32F405 OSF0 UART stream -> Raspberry Pi 4 serdev -> Linux IIO raw and
buffer reads.

Environment recorded during testing:

- Raspberry Pi 4
- kernel `6.12.75+rpt-rpi-v8`
- OSF GREEN UART OSF0 stream

Observed IIO devices:

- `osf-accel`
- `osf-gyro`
- `osf-magn`
- `osf-temp`

No OSF oops, panic, or call trace was observed in that smoke.

This smoke does not claim production timestamp correlation or hardware
certification.
