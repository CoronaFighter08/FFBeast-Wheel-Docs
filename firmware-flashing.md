# Wiring / Flashing Controller

Controller wiring and flashing is best left to the main docs, as it explains everything in great detail and needs no further comment.

{% embed url="https://ffbeast.github.io/docs/en/connection_odrive.html" %}

{% embed url="https://ffbeast.github.io/docs/en/software_firmware_flashing.html" %}

_<mark style="color:$danger;">**REMEMBER TO NEVER TRUST WIRE COLOR CODING!**</mark>_ <mark style="color:$danger;"></mark><mark style="color:$danger;">Always match connections by pinout and names, never trust wire colors from images or videos as they can be different depending on what you have.</mark>

***

## ODrive DFU Application

Developed by EulerOliveira from the FFBeast community server, the ODrive DFU application helps in setting the controller board into DFU mode for flashing, something a lot of people face trouble with. Feel free to check it out incase you're facing similar issues!

{% embed url="https://github.com/achavevirou/odrive_dfu/blob/main/README.en-us.md" %}

***

## ODrive Backflow Protection (Relay Wiring)

<mark style="color:$warning;">(UPDATE: Some members have stated that the relay method can cause more harm than actual good. I don't have the relays installed so I can't speak as to how it is with or without them. I recommend you read the discussion thread in the Discord before deciding whether to go ahead with it!)</mark>\
\
Another helpful piece of information shared by EulerOliveira. As the ODrive controller is susceptible to damage due to power backflow from spinning the wheel (and hence the motor) excessively while the whole thing is powered down, cheap relays can be wired up between the motor and the controller to cut off the connection when there is no power.

{% columns %}
{% column %}
<figure><img src=".gitbook/assets/image (10) (1).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
<figure><img src=".gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

Remember to use relays which are driven using 5V, and to wire up the motor to the NO (normally open) terminals so that the circuit is broken when the board is unpowered!
