---
cover:
  light: ../.gitbook/assets/controller_cover.png
  dark: ../.gitbook/assets/controller_dark.png
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Controller

{% hint style="info" %}
The FFBeast firmware is currently compatible with controllers which work with ODrive 3.6, including various remixes such as ODESC and XDrive. For a full list of compatible controllers, visit the [official docs](https://ffbeast.github.io/docs/en/hardware_controller.html) for more info. We will only be focusing on the Single Axis ODESC V4.2 style controller in this guide due to its popularity within the wheel building community.
{% endhint %}

## Why The ODESC V4.2 Schematic Design?

This guide is centered around the ODESC V4.2 Design due to its popularity (almost all FFBeast wheels use this controller board, and many pre-made enclosures are built around it), relatively low cost compared to other boards, and its availability. It's also compact and features a built-in heatsink making it easy to integrate.

The [Makerbase XDrive MINI](https://makerbase3d.com/product/makerbase-xdrive-mini-high-precision-brushless-servo-motor-controller-based-on-odrive3-6-with-as5047p-on-board/) is an ODrive 3.6 board which has a similar design. It has been successfully used in multiple builds.\
\
The no-name clone boards from Aliexpress and similar sites _should_ also work, however the risk of receiving faulty components will be increased. The final decision is up to you ;)

You are, of course, free to use other ODrive 3.6 controller boards. Make sure to check the official docs for the official compatibility list before doing so.

## Should I go for the 24V or 56V version?

The listed voltage value is simply the maximum operating voltage of the board and it won't matter if you drive your motor at 24V using a 56V board. The decision is up to you!

## Protecting Your Controller

One important thing to keep in mind about these controllers is to be careful of potential damage from current backflow. During use of the FFBeast wheel, rotation of the wheel (and subsequently the motor) causes it to essentially become a generator, sending energy into the board. When powered, this excess current is dumped into the braking resistor, however when unpowered the backflow can potentially damage your ODrive board from excessively spinning the wheel.

For those who are worried about someone in their home potentially spinning their unpowered wheel and damaging the controller, cheap relays can be installed between the motor and the controller to prevent backflow when unpowered. [The wiring and setup for this is mentioned here.](../firmware-flashing.md#odrive-backflow-protection-relay-wiring)

