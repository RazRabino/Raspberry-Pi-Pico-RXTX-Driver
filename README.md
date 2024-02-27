<div align="center">

# Raspberry Pi Pico RXTX Driver

RXTX (based on flysky radio module) driver for raspberry pi pico (pico c/c++ sdk projects).
this code libraray developed as part of my main project "FCP" (autonomous flight controller project),
it can be used for other projects thats need radio transmitter - receiver data management.
based on the FlySky i6x and FlySky FS-iA6B.

Hardware:

[Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/) •
[FlySky i6x](https://www.flysky-cn.com/fsi6x) •
[FlySky FS-iA6B](https://www.flysky-cn.com/ia6b-canshu)

</div>

<div>

# Example Of Use

```c++
RXTXdriver rxtx_driver;
RXTXdata rxtx_container;
rxtx_driver.read_data(rxtx_container);
yaw_servo.pwmservo_write_micros(yaw_servo_pin, (rxtx_container.ch4));
```

</div>
