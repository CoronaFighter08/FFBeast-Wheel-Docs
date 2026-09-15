# Tips, Tricks & Troubleshooting

Check the menu on the right to jump to different sections on this page!

## Troubleshooting

Almost all the issues I've seen in the Discord server are related to the encoder in one way or another. Losing FFB over time, wheel not centering correctly, hard stops not working, the wheel spinning like crazy, etc.&#x20;

Check your mounting method to make sure the motor's shaft is tightly secured and can't slip - use a marker to mark a point on the shaft and see if it moves while you play. If you're using belts or gears, ensure they aren't slipping or skipping. CHECK YOUR CPR!!! There have been cases of magnetic encoders having different PPR values than the one listed in the product description.

If you're using an ODESC 4.2 board with rotary encoders, you might have to add pullups and remove capacitors. Join the Discord and use the search feature to look for the guide.

Your wheel shutting down while you're fighting the FFB is a sign of an underpowered PSU. If it shuts down during fast movements, it's a sign of the braking resistor value being too low.

If your troubleshooting attempts are unsuccessful, don't worry! You can always ask for help in the Discord and someone will answer - assuming you do it correctly. Speaking of which:

## Asking For Help (The Correct Way)

"my wheel goes crazy when i hit the right endstop, help"

This tells us absolutely nothing. At the bare minimum you should be providing details of your motor, motor mounting method, encoder, encoder mounting method and any details regarding it (gear teeth, ratio, etc) and screenshots of your settings. A video is even better. Don't expect to receive help if you can't describe your problem.

***

## Don't Rip Your USB-C Port Off (Please)

Go ahead, but you'll need to be good at soldering. The USB-C ports on the controllers are mounted at a 90-degree angle for whatever reason, so they are REALLY easy to rip off along with the pads.

{% embed url="https://www.printables.com/model/1435932-odrive-mini-usb-c-port-guard-reinforcement-bracket/related" %}

I recommend using this USB-C guard unless you have some other method of strain relief or a separate USB port integrated in your build's enclosure. However, if you have already ripped it off, you'll need to solder a spliced USB cable directly to the pads of your controller. An image below shows where to solder the data lines and ground. <mark style="color:$danger;">DO NOT CONNECT THE 5V+ WIRE.</mark>

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>



## Tips For Assembly

Here are some cool tricks I learned from others or from personal experimentation:

* If the screws on the back plate of the hoverboard motor are stuck, hit them with a hammer. Literally. I took a bolt with a diameter slightly less than the one of the screws, placed that bolt on the face of the screw and hit the bolt with a hammer. Multiple times. It loosened them right up!
* 🍞🍞🍞 If you need to remove the inner bearing to drill a hole for the magnetic encoder, you can use bread to stuff the portion behind the bearing and force it out. I'm not joking, it apparently works. I've personally never tried it so please join the Discord and search for peoples' experiences with this method cause I'm not responsible if you end up with a bread-logged bearing.
* Remove the phase wires before you drill through the shaft. You will 100% drill straight through and cut them. Route some string through the hole once you're done, tie it to the phase wires and use it to pull the wires back through the shaft.

## Heat Management?

Motors get hot during use. Less powerful motors (less than 30mm magnet / stator length) get even hotter. How much is too hot?

You only need to start getting worried once you cross 70 degrees Celsius as at around 80 degrees you can start to permanently damage the magnets. A way to fix this is ventilation. You can drill large holes in the front and back faces of the motor to allow for this. Using a fan to suck air through said holes is even better. There are multiple interesting examples of this in the Discord server.

Just be careful while drilling holes in the front as that's also where you mount your wheel to and overdoing it could lead to your wheel being broken off.

## Power Supply

24V 20A is the sweet spot and what everyone uses (and yes, it's fine for drifting as well). Higher voltage will increase the RPM too much, and lower voltage results in a sluggish feeling wheel.
