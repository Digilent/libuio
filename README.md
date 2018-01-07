# libuio

A user-space library for interfacing with generic uio devices. 

UIO devices are assigned a device number upon registration with the kernel. A UIO device can have multiple maps or partitions inside of it as well, and each map is assigned its own number inside the device. Informaiton about these devices can be found in `/sys/class/uio`.

Using the UIO device number, the UIO map number, and this user-space library, a user can map and unmap the hardware into physical memory in an easy way by using this library. 

This library can be used in a standalone format, but is also used with [libgpio](https://github.com/mitchellorsucci/libgpio) and [libpwm](https://github.com/mitchellorsucci/libpwm) for easy control of GPIO and PWM devices that exist in an FPGA.

For examples of how to use this library, please reference our pwm and gpio libraries linked above, and check out our [pwm](https://github.com/mitchellorsucci/pwmdemo) and [gpio](https://github.com/mitchellorsucci/gpioutil) demo programs.
