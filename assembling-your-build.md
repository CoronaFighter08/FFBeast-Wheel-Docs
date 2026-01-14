---
description: This is it! This is what we've been waiting for!
---

# Assembling Your Build

Once you've read through the [official docs](https://ffbeast.github.io/docs/en/wheel.html) and have decided which parts & design you intend to go with based on the [subpages](parts-+-tools-required/) linked above, it's time to assemble the build!

{% stepper %}
{% step %}
### Remove Motor Backplate

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

There are six phillips head countersunk screws holding the back plate of the motor on. They are prone to stripping so be extremely careful when unscrewing them. Mine were stuck, so I used a large bolt I had laying around, placed it on top of the screws and gave it a few hard whacks with a hammer which loosened them right up. The backplate should slide right off with a bit of force.
{% endstep %}

{% step %}
### Pulling The Stator Out

Depending on your magnet size, the stator can be extremely difficult to pull out. It's suggested you place the place the motor on your floor, hold it using your feet and then try holding the shaft as tightly as possible and pulling hard. Pliers to grip the shaft also help a lot here.

<figure><img src=".gitbook/assets/FFBeast Motor Pull.gif" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Removing Wires (If Drilling Motor Shaft)

If you intend to drill a hole through the motor shaft to pass a magnetic encoder or slipring's wire through (or to use the bike spoke encoder mounting method) then it's highly recommended you remove the wires to prevent damage to them.

<details>

<summary>Remove the hall effect sensors. </summary>

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption><p>The hall effect sensors are not used in the FFBeast build, so they can be removed along with their wires.</p></figcaption></figure>

</details>

<details>

<summary>Remove the thick insulation &#x26; crimped ends.</summary>

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption><p>These need to be cut off, being careful not to damage the wires underneath.</p></figcaption></figure>

</details>

<details>

<summary>Pull the wires through.</summary>

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption><p>Using pliers to firmly grip the wires, pull them from the bottom hole of the motor shaft. Make sure it doesn't pull and cause stress on the joint between the copper windings and the wire!</p></figcaption></figure>

</details>
{% endstep %}

{% step %}
### Drilling The Shaft

If you plan to drill a hole through the motor shaft, make sure you've removed the wires first. Whichever method you choose to drill it, whether it be a hand drill, a drill press, or even a lathe, I recommend you place something like a piece of paper with a hole cut out on top with the shaft poking through to prevent metal shavings from dropping into and getting stuck in the motor windings.

The shaft is made from hardened steel, so just look up how to drill through that stuff since I'm not qualified to tell you this (I didn't drill through mine) 😝
{% endstep %}

{% step %}
### Drilling The Mounting Holes

The holes for mounting your wheel, spacer or quick release are usually drilled through the inside of the motor as depending on your wheel's front design, it might not allow a flat surface while the inside does.

If you plan to go with the common 70mm M5 bolt pattern, I recommend printing this out:

{% embed url="https://www.printables.com/model/1229289-70mm-m5-bolt-pattern-drill-guide" %}

It can be inserted in the front bearing to align the mount and you can then drill through the front of the motor. It should be quite easy as the casing is made from aluminium.&#x20;

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

I would highly recommend you use paper, tape or literally anything to prevent metal shavings from sticking to the magnets as it could cause issues once you reassemble the motor. I made a paper "bowl" with a hole in the middle which caught the metal shavings as I drilled and could be easily removed later and disposed of.
{% endstep %}

{% step %}
### Mount The Wheel / Spacer / Quick Release

This one is pretty self explanatory. Hold the thing you want to mount on the front of the motor and screw your bolts in from the inside. Use either countersunk or button head bolts as those with large enough heads could potentially grind against and damage the copper windings. I personally haven't seen that happen to anyone in the community discord but you never know!
{% endstep %}

{% step %}
### Motor Reassembly

Essentially the opposite of the disassembly. If you're using a front mounted magnetic encoder or have any wires to pass through the shaft, do it now. Hold the motor casing with your feet as you gently lower the stator back into it. Be careful to ONLY hold it by the shaft as it will suddenly snap back in (trust me, you don't want your fingers to be in the way).

The back plate can be slid back on and screwed in as normal.
{% endstep %}

{% step %}
### Test Your Encoder

Get your ODrive board. Connect it via USB to your computer and give it external power (the boards shown in [controller.md](parts-+-tools-required/controller.md "mention") can't be powered off the USB connection alone). Flash the FFBeast firmware onto the board. [firmware-flashing.md](firmware-flashing.md "mention"). Unpower the board and connect your encoder, making sure you do NOT wire up the motor. Power the board back up and apply the correct settings for your encoder through the wheel setup app. Forces should be disabled.

Open any app or game which can display your wheel position. Hold the motor in your hand and give it a spin. If everything is working fine, you can continue with mounting everything!
{% endstep %}

{% step %}
### Mounting Your Motor

Depending on the motor mount you decided to use (examples given in [motor-mounting.md](parts-+-tools-required/motor/motor-mounting.md "mention")), it may require some assembly beforehand. Once that's done, mount your motor and ensure the shaft can't slip in the mount. You can now connect the motor to the controller and test everything at low power to make sure the force feedback is working as expected, as your electronics are easy to access at this point.
{% endstep %}

{% step %}
### Mount Your Electronics

It's recommended you don't leave your electronics laying out as it increases the risk of accidental short circuits from foreign objects, electrocution, and in general the controller getting dusty. Even if you don't have an enclosure to hide everything, you should atleast have a mount to have your controller and braking resistor properly attached to. If you intend to connect anything else like backflow protection relays, internal USB hubs, or more, then you can do so now.
{% endstep %}

{% step %}
### Enclose Everything (If You Intend To)

If you have an enclosure you intend to install, it's time to do it!! Once everything has been tested and any issues have been rectified, there's nothing more left to do than to make everything look neat. Zip tie loose wires and tuck them in. Make sure your mount is properly tightened in the position you want it in. Give the whole thing a good tug to make sure your setup won't go flying off your rig or desk. Doesn't hurt to check, you know?
{% endstep %}

{% step %}
### Have Loads Of Fun

As someone who went from a 2.2 Nm Logitech G29 to a (supposedly, I've never set the force to 100%) 15 Nm capable direct drive wheel for even cheaper, I can personally attest that this is one of the most entertaining DIY projects I've ever made. The whole point of these "community docs" was to share all the info in one place which I would have personally found useful to have when I was building my wheelbase. I hope that you found this useful and have lots of fun using your own DIY FFBeast wheel!
{% endstep %}
{% endstepper %}
