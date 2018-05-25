# 4.5 Power Supply Configurations

In most cases, there is no need to worry about the GoGo Board’s power supply. However, when a non-5v motor is used or when many power hungry output devices are connected, special care will be needed to make sure the GoGo Board functions properly.

## Voltage

Each output port on the GoGo Board delivers 5 volts by default. However, the GoGo Board has an auxiliary power source connector if other voltages are needed. This voltage must be between 3-12v. There is a jumper next to the on/off switch that can be used to send either 5 volts or the auxiliary voltage to the output ports. The illustration below shows how to use this jumper.

{% hint style="danger" %}
**Caution** - The power source for all four output ports are internally connected. Therefor, all ports will supply the same voltage. Devices that require different voltages cannot be used at the same time. You **cannot mix** 5-volt and 12-volt devices, for example.
{% endhint %}



![](https://lh5.googleusercontent.com/SHbmNlPESDTTMyw2BZG4frA7Eh9qpqbyXuhzq_1CP_L8NVT9PjDEyYFsOXyizw669OvV_kHvLw_f5RuAkTz0hnrsOjQC2W5tsahYJnt9O1KZvRLIiFl2DHnxdtpKMNUbd-LZp2LT)

## Current {#current}

In some cases when using many output devices, the GoGo Board many need to be supplied with a higher current source. A common problematic scenario is when trying to drive many motors using power only from a computer’s USB port. Most computer USB ports can supply only 500 mA. Power banks or phone chargers with a mini USB cable can usually supply 1,000 - 2,500 mA. Alternatively, the GoGo Board also has a 5v power supply connector \(see illustration below\). This connector can be used with other 5v power sources such as batteries or wall adapters.

