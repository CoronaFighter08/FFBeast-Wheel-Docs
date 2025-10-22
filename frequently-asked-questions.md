# Frequently Asked Questions

Frequently asked questions answered here. If you have any suggestions, send me a DM on Discord @ coronafighter (or just ping me in the FFBeast Discord!).

<details>

<summary>Which tools do I need for this build?</summary>

Like many other DIY projects, this mainly depends on how you go about building it. However the most common tools used are a drill, soldering equipment, screwdrivers, and glue. You'll also most likely be using 3D printed parts, allen keys, and maybe even a lathe. In a pinch you can rent these tools or get any drilling work done from a workshop.

</details>

<details>

<summary>What's the best motor to use?</summary>

You'll get the best price to performance with a 6.5 inch diameter hoverboard motor with 30mm magnet / stator height along with 5 strand winding. You can find more info on finding these motors here: [#how-to-get-the-best-motor](parts-+-tools-required/motor/#how-to-get-the-best-motor "mention")

</details>

<details>

<summary>Which encoder solution should I go with?</summary>

It's recommended to go with a magnetic encoder mounted using something like Viih's encoder mount ( [#viihs-magnetic-encoder-mount](parts-+-tools-required/encoder/mounting-connection.md#viihs-magnetic-encoder-mount "mention")). However if you don't want to drill through the hard steel motor shaft, an [optical encoder driven using belts](parts-+-tools-required/encoder/mounting-connection.md#belt-driven-encoders) will also work perfectly fine.

I wouldn't recommend gear driven encoders as they can have issues with backlash, and the bike spoke method is not worth the drilling effort because you could just use a magnetic encoder at that point.

</details>

<details>

<summary>Which power supply should I go with? Isn't my motor rated for 36V?</summary>

It's recommended you go with a 24V 20A power supply. While you could use higher voltage, both the power supply and the ODrive board (56V version) will cost more. Since there's a lock on the motor's power output, the motor can only pull a max of 15A at 24V. So a higher voltage will **only increase your RPM**, **not your torque**. The RPM at 24V is considered more than enough, even for drifting. The 5 ampere headroom is so your power supply doesn't shutdown :)

</details>

<details>

<summary>Should I go with a 24V or 56V ODrive board?</summary>

Since the 56V version usually costs more, just go with the 24V one. That's the max voltage it's recommended you run your motor at anyways. Since there's a lock on the motor's power output, the motor can only pull a max of 15A at 24V. So a higher voltage will **only increase your RPM**, **not your torque**. The RPM at 24V is more than enough!

</details>

<details>

<summary>Do I need to buy a FFBeast firmware license?</summary>

Not necessarily, unless you want to run pedals or other connections through the ODrive board's GPIO and access to a couple more settings. It's mostly to support the developer!

</details>

<details>

<summary>Is there any way to protect my build from dying? :(</summary>

Consider having a case to protect your electronics from the environment (and other foreign objects). Use [relays between the motor and the ODrive board](parts-+-tools-required/controller.md#protecting-your-controller) to prevent power backflow damage. An automotive fuse between the power supply & board wouldn't hurt either.&#x20;

Also consider using a USB extension or a 3D printed brace for the USB port on your ODrive board, as some people have accidentally ripped theirs off. Ouch...

</details>

<details>

<summary>I'm facing an issue with my build. What do I do?</summary>

Check out [troubleshooting-faq.md](troubleshooting-faq.md "mention") first. If a solution can't be found there, feel free to ask for help in the Discord server! The invite button is in the top right of this page.

</details>
