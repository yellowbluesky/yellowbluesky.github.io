---
layout: post
title:  "MSI B350M Mortat Arctic Output Impedance"
date:   2020-01-12 12:05:15 +1100
categories: outputImpedance motherboard computer electrical measurement
---
TL;DR: The MSI B350M Mortar Arctic motherboard has an output impedance of around 80 Ohms, on both its front panel and rear panel headphone out jacks.

I'd always known the headphone output of this motherboard to be sub par, given its bargain pricing of $130 when new. I don't even use it, instead using a trusty Fiio E10K as a DAC to my various other amps. This set of measurements is just for an academic view of things


## Test setup

Two sets of measurements were taken: one fron the front panel and one from the rear panel. A 1 kHz tone was generated using this website (https://www.szynalski.com/tone-generator/). Volume on the device and website were both increased to their maximums.

The front panels and rear panels were connected to the measurement platform with a 3.5mm interconnect.

Measurements were taken with an ADALM2000. More information can be found [on their website](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalm2000.html#).

The ADALM2000's analog inputs have only a 50 kOhm input impedance, so the signal is first buffered using LF353 op-amp before beign fed into the ADALM2000's oscilloscope inputs.

A 10 Ohm resistor was used as the load.

## Results
# Rear panel
The first set of measurements comes from the rear panel.


Unloaded:
[![Rear panel unloaded oscilloscope trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearNoLoadBufferedScope.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearNoLoadBufferedScope.png)
An unloaded voltage of 3.5V is a tad on the low side, but is still servicable for the low impedance gaming headsets that MSI expected people to pair with this motherboard.

Loaded:
[![Rear panel loaded oscilloscope trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearLoadBufferedScope.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearLoadBufferedScope.png)
Note the changed vertical scale in the second scope trace, visible in the lower left corner. Output voltage drops to 0.385V.

This computes to an output impedance of approximately 80 Ohms.

# Front panel

Unloaded:
[![Front panel unloaded oscilloscope trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontNoLoadBufferedScope.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontNoLoadBufferedScope.png)

Loaded:
[![Front panel loaded oscilloscope trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontLoadBufferedScope.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontLoadBufferedScope.png)

Output impedance computes to 85.56 Ohms.

## Conclusion

An output impedance of over 80 Ohms is rather poor, but what was I expecting for a budget motherboard running only an ALC892 codec.

## Other

A spectrum analyzer was also run on the front panel and rear panel. I choose to include them here and not the main results section, as:
- Measurement setup is rather noisy: long unshielded interconnects and jumper wires
- ADALM2000 analog inputs only have a 12 bit accuracy

Rear panel:
[![Rear panel unloaded spectrum analyzer trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearNoLoadBufferedSpectrum.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/rearNoLoadBufferedSpectrum.png)

Front panel:
[![Front panel unloaded spectrum analyzer trace]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontNoLoadBufferedSpectrum.png)]({{site.baseurl}}/images/2020-01-12-B350mMortarArcticOI/frontNoLoadBufferedSpectrum.png)

If those numbers are to be believed (which I don't), then there is only about 60dB of SNR, which is also fairly poor.

I am aware of the constantly changing vertical scale on my scope traces, I apologize. Future posts will not have this oversight from me.