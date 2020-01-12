---
layout: post
title:  "MSI B350M Mortat Arctic Output Impedance"
date:   2020-01-12 12:05:15 +1100
categories: outputImpedance motherboard computer electrical measurement
---
TL;DR: The MSI B350M Mortar Arctic motherboard has n output impedance of 85.5 Ohms, on both its front panel and rear panel headphone out jacks.

I'd always known the headphone output of this motherboard to be sub par, given its bargain pricing of $130 when new. I don't even use it, instead using a trusty Fiio E10K as a DAC to my various other amps. This set of measurements is just for an academic view of things


# Test setup

Two sets of measurements were taken: one fron the front panel and one from the rear panel. A 1 kHz tone was generated using this website (https://www.szynalski.com/tone-generator/). Volume on the device and website were both increased to their maximums.

Measurements were taken with an ADALM2000. More information can be found [on their website](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalm2000.html#).

The ADALM2000's analog inputs have only a 50 kOhm input impedance, so the signal is first buffered using LF353 op-amp before beign fed into the ADALM2000's oscilloscope inputs.

Two measurements were then taken from the output:

* One unloaded measurement
* One measurement across a 10 Ohm resistor acting as load

# Results

Unloaded voltage was recorded as being 2.736 Volts on average, across 3 measurements. 

Loaded voltage was recorded as being 0.636 Volts on average, across 3 measurements.

This computes to an output impedance 33.02 Ohms

# Conclusion

This is a very very poor result. An output impedance that high will significantly color the sound of headphones with an impedance lower than 264 Ohms, essentially disallowing the use of nearly all portable headphones.

# Other
When used with an IEMatch to correct the output impedance fault, the 