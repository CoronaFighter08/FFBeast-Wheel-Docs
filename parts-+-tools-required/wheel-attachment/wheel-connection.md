---
description: Slip rings, coiled cables, & wireless setups!
---

# Wheel Connection

If your steering wheel has paddle shifters, push buttons, encoders, etc, you're going to need a way to hook them up to your computer. The buttons and switches themselves are usually connected to a microcontroller, such as an Arduino, ESP32, RPI Pico, etc, leaving you with the USB connection left to handle.

Shown below are a few different ways members of the FFBeast community have handled this particular issue:

## Wired Connection (Coiled Cable)

{% columns %}
{% column %}
<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
The simplest and arguably the most reliable solution. Can be bought pre-made with GX-16 (or similar) connectors from places like Aliexpress or made yourself using RJ9 telephone cords or similar coiled cables available from common appliance or electrical stores.

Make sure to get a suitable length depending on what your steering limits will be. It's advised to wrap your coiled cable around your steering wheel shaft to prevent it from flopping about everywhere :)
{% endcolumn %}
{% endcolumns %}

***

## Slipring Connection

{% columns %}
{% column %}
<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
A slip ring can be used to connect your wheel's controller to your PC in a clean and "invisible" way. Allowing your wires to run through your hoverboard motor and not get tangled up, it requires drilling through the motor shaft and some mounting solution. However the end result is a clean, wireless wheel connection which allows for an infinite wheel rotation as there are no wires to get wrapped up.
{% endcolumn %}
{% endcolumns %}

{% embed url="https://www.printables.com/model/1282058-hoverboard-motor-encoder-and-slip-ring-mount-for-f" %}

***

## Wireless Controller

{% columns %}
{% column %}
<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
While not being recommended due to potential connection issues and other hassles like charging, wireless wheel connections are the cleanest way. Using cheap wireless gamepad boards from Aliexpress, ESP32 boards (or even a disassembled Xbox controller!), members of our community have successfully built setups  with wheels running wirelessly on battery.
{% endcolumn %}
{% endcolumns %}

***

## Which Method Should I Use?

Each method has its pros and cons. Wired using coiled cables is the easiest, however some don't prefer the rotation limit from the wire and are distracted by it. Slip rings are used by most commercially available wheelbases, however cheap ones can go bad quickly and it requires drilling into your hoverboard motor shaft to route the wires through it (not to mention the fact that you'll need a 3D printed mount to hold the slipring). Wireless is the cleanest way, however some users face connection issues, not to mention the hassle of managing your battery to ensure your wheel doesn't die in the middle of a race.

I'd personally recommend going wired, but in the end it's your build after all. It's entirely up to you!
