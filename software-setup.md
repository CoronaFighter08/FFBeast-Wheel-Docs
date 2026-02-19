---
description: A guide on setting up your wheelbase.
---

# Software Setup

The following guide doesn't list what each setting does - for that, go to the official docs page listed below. What it does do however is provide step by step instructions for setting everything up in the correct order.

It also assumes that you've fully completed the hardware part of your build and have flashed the firmware. Make sure your wheel is properly mounted / clamped to your rig or desk and can not move, as you'll be testing the force feedback as well. Plug your wheel's power and usb in, open the FFBeast setup app and let's begin!

{% embed url="https://ffbeast.github.io/docs/en/ffbeast_setup.html" %}

***

{% stepper %}
{% step %}
### Effects Menu

Set motion range to 90 degrees to make checking softstops easier later. Static dampening should be set to 0% and total effect strength at 100%.


{% endstep %}

{% step %}
### Controller Menu

Ensure all checkboxes at the top are unticked, especially the one labelled "Enable forces". Your P and I gains should be at their defaults of 10 and 100 respectively. Don't touch them unless you know what you're doing - they are best left at the default. Calibration magnitute should be at 5% with its speed at 100%. These usually don't have to be changed either.

Set your power limit to 5-10% for now for testing.


{% endstep %}

{% step %}
### Set Your Pole Pairs

The number of pole pairs is simply the number of magnets in your hoverboard motor drivided by two. For most motors it's 15 (since they have 30 magnets).


{% endstep %}

{% step %}
### Set Your Encoder CPR

This is the part most people mess up, and can result in multiple issues. Make sure you get this right!

The CPR value you have to insert is your encoder's PPR value (given in the datasheet) multiplied by 4. If you have any gear reductions, you have to factor that in aswell!

For example, if I have a 1000 PPR encoder, I'll insert 4000 (4 x 1000) as my CPR. However if my encoder is attached to the motor through a 2:1 gear reduction (encoder spins twice as fast as the motor) then my CPR will be 8000.


{% endstep %}

{% step %}
### Save & Test Encoder

Click the "Save and reboot" button. Open some game or joystick tester to check and see if your encoder is working properly by spinning the wheel. If your wheel shows up spinning the wrong way, tick the "Invert joystick output" checkbox and check again to see if it's fixed. If your wheel is spinning less or more in-game than you actually are, that's a clear indication that your CPR value is incorrect.


{% endstep %}

{% step %}
### Test The Motor

<mark style="color:$danger;">!!! Make sure your wheelbase is properly clamped down and can not move !!!</mark>

Once your encoder is properly set up, tick the "Enable forces (requires reboot)" checkbox and then click "Save and reboot". Once your controller reconnects, your motor should do a small wiggle during the calibration sequence. That is normal.

Now assuming you set your motion range and power limit correctly before, you can now turn your motor 45 degrees either way from center. Once you reach the limit, the motor should slightly resist your motion to further turn it away from center. That means it's working. However if the motor tries to pull the wheel even further from the center and starts spinning uncontrollably, you need to tick the "Invert force output" checkbox before saving and rebooting.

You can now increase your motion range to a more acceptable value like 900 or 1080 degrees.

Remember to save and reboot once you're happy as the next step might cause a few restarts of your wheel which can cause you to lose your settings if not saved.


{% endstep %}

{% step %}
### Braking Resistor Limit

The point of the braking resistor is to get rid of excess energy from you spinning the wheel and to turn it into heat instead of sending it back to your power supply and causing it to shut down. Getting the value right requires a bit of trial and error.

Start with a small value - around 5 to 10% is good. Then try mimicking yourself playing a game and turn the wheel quickly / sharply from left to right, making rapid movements. If your power supply shuts down, add 5% more to the limit value and try again. Once your power supply stops shutting down, the value you're left with is the one you want to use!


{% endstep %}

{% step %}
### Static Dampening

The static dampening setting, listed in the Effects tab, can help reduce wild oscillations of your wheel. You only want to use around 2-3% as a higher value will begin to reduce the actual effects you want to feel from the game. I personally only use a value of 1%.


{% endstep %}

{% step %}
### Increase Power Limit

Now that everything is setup up and working, you can increase your power limit! If you have a PSU with a lower current rating, you might have to limit the power to prevent it from shutting down.

When increasing your power limit, taking into consideration the fact that you are increasing the maximum possible output of a direct drive wheel which can possibly reach a peak torque of 15 Nm. Make sure your wheel is properly attached to your table or rig before doing so.

I recommend starting with a lower power limit if this is your first time using a DD wheel so that you can get a feel for it first. Once you want the full experience, I recommend setting a high power limit and then limiting the strength through the ingame gain value - this prevents clipping of the force feedback.


{% endstep %}

{% step %}
### Have fun!

Need I say more? :)
{% endstep %}
{% endstepper %}
