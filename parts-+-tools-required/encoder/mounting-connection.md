---
description: Showcasing & comparing different encoder mounting solutions.
---

# Mounting / Connection

## [Viih's Magnetic Encoder Mount](https://www.printables.com/model/934160-ffbeast-encoder-assembly)

Made for the MT6701 18x15mm magnetic encoder, this 3D printed mount by [Viih](https://www.printables.com/@Viih_341714) from the FFBeast Discord allows the encoder to be seated in the hoverboard motor shaft and stay stationary while a magnet positioned above it rotates along with the housing of the motor.

{% embed url="https://youtu.be/rZpp99V58DY?si=DXhbk_hLk9J9Ninh" %}

| Pros                                              | Cons                                                 |
| ------------------------------------------------- | ---------------------------------------------------- |
| Budget friendly.                                  | Difficulty in drilling hole in hard steel shaft.     |
| No contact, meaning no wear. Will last "forever". | Hole needs to be centered, some people mess this up. |
| Precise encoder mounting.                         |                                                      |

***

## [tig33r's Magnetic Encoder Mount](https://www.printables.com/model/1380474-magnetic-encoder-mount-for-hoverboard-wheel-motor)

A remix of Viih's encoder mount, this 3D printed mount by [tig33r](https://www.printables.com/@tig33r_3322973) from the FFBeast Discord allows for either a MT6835 or MT6701 magnetic encoder to be positioned in a similar fashion to Viih's mount. The main difference with this one is that **it works with an off-centre hole drilled in the axle**.

{% embed url="https://www.youtube.com/watch?v=VyxdB34GASg" %}

| Pros                                              | Cons                                             |
| ------------------------------------------------- | ------------------------------------------------ |
| Budget friendly.                                  | Difficulty in drilling hole in hard steel shaft. |
| No contact, meaning no wear. Will last "forever". |                                                  |

***

## Gear Driven Encoders

Usually paired with OMRON style encoders, driving your encoder via gears is a method which requires no extra hardware, provided you have a 3D printer and heat resistant filament on hand. Examples of gear driven encoders are [this](https://www.printables.com/model/981504-hoverboard-ffbeast-openffboard-ffb-sim-wheel-encod) and [this](https://www.thingiverse.com/thing:6664358).

<figure><img src="../../.gitbook/assets/image (2) (1) (1).png" alt="" width="375"><figcaption><p>Credits: <a href="https://www.thingiverse.com/diegomlino"><strong>diegomlino</strong></a> <strong>on Thingiverse</strong></p></figcaption></figure>

| Pros                                        | Cons                                            |
| ------------------------------------------- | ----------------------------------------------- |
| No drilling required, easy to assemble.     | Increased mechanical wear and tear.             |
| No extra hardware if you have a 3D printer. | Potential for gear skipping and backlash.       |
| Gearing allows for CPR increase.            | Difficulty in aligning gears to mesh correctly. |

***

## Belt Driven Encoders

Belt drive is commonly used by those with OMRON style encoders as it allows for easier assembly (no difficult drilling involved) while removing the gear alignment issues of gear drive.

<figure><img src="../../.gitbook/assets/image (3) (1) (1).png" alt="" width="387"><figcaption><p>Credits: <a href="https://cults3d.com/en/users/Olukelo/3d-models">Olukelo</a> on cults3d</p></figcaption></figure>

| Pros                                        | Cons                                      |
| ------------------------------------------- | ----------------------------------------- |
| No drilling required, easy to assemble.     | Slight mechanical wear overtime.          |
| No extra hardware if you have a 3D printer. | Potential for skipping if belt is loose.  |
| Gearing allows for CPR increase.            | No "one size fits all" mounting solution. |

***

## Bike Spoke Method (OUTDATED)&#x20;

{% columns %}
{% column %}


<figure><img src="../../.gitbook/assets/image (4) (1).png" alt="" width="188"><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
Superseded by the belt drive and Viih mount, this method uses a bike spoke attached to the motor's front housing running through a hole in the motor shaft to the back, before connecting to the encoder. An OMRON style encoder needs a simple connector while a magnetic encoder requires a bearing to hold the magnet at the end of the shaft steady to remove wobble.

Now outdated, there are no real benefits from mounting and connecting your encoder this way, and the effort required can instead be used to prepare a Viih mount or belt drive system.
{% endcolumn %}
{% endcolumns %}

| Pros                                                                                 | Cons                                                                                  |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- |
| Clean encoder mount (no protruding belts, gears, etc).                               | Tendency for bike spoke to loosen and start slipping.                                 |
| No 3D printed parts necessarily required (atleast if using the OMRON style encoder). | Spoke rubs against wires in the motor shaft and requires a cover.                     |
|                                                                                      | Requires drilling into the hard steel shaft which can instead be used for Viih mount. |
|                                                                                      | Requires a bearing setup to hold the spoke steady for magnetic encoders.              |

***

## Which Mounting Method Is Best For Me?

This depends on your budget, encoder type, tools on hand, etc. For general users, the Viih mount is recommended. For those willing to spend a little more on an OMRON style encoder and not wanting to drill into the hard steel motor shaft, the belt driven encoder is the next best solution!
