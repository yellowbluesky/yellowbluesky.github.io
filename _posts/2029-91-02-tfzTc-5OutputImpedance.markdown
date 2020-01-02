---
layout: post
title:  "TFZ Tc-5 Output Impedance Measurement"
date:   2019-12-14 12:05:15 +1100
categories: outputImpedance phone electrical measurement
---
TL;DR: The TFZ TC-5 has an output impedance of 33 Ohms.

The TFZ TC-5 is a USB C DAC and amplifier combo. I chose it because of its good specifications on paper, and its looks which would match the rest of my portable audio setup (IEMatch + silver Litz cable).

Oh first demo of it, I noticed that mt IEM's (B400) took on a very unnatural bright tilt to the sound. Suspecting an isssue with the output impedance of the TC-5, I measured them.

#Test setup

The TC-5 was attached to me Redmi Note 7 Pro. A 1 kHz tone was generated using this website (https://www.szynalski.com/tone-generator/). Volume on the device and website were both increased to their maximums.

Two measurements were then taken from the output:

	* One unloaded measurement
	* One measurement across a 10 Ohm resistor acting as load

#Results

Unloaded voltage was recorded as being 2.736 Volts on average, across 3 measurements. 

Loaded voltage was recorded as being 0.636 Volts on average, across 3 measurements.

This computes to an output impedance 33.02 Ohms

#Conclusion

This is a very very poor result. An output impedance that high will significantly color the sound of headphones with an impedance lower than 264 Ohms, essentially disallowing the use of nearly all portable headphones.

#Other
When used with an IEMatch to correct the output impedance fault, the 