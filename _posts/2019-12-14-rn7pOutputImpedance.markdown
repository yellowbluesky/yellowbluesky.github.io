---
layout: post
title:  "Redmi Note 7 Pro Headphone Output Impedance"
date:   2019-12-14 12:05:15 +1100
categories: outputImpedance phone electrical
---
TL:DR; The Redmi Note 7 Pro (violet) have an output impedance of 10 Ohms. This value is flat across the audible range.

I took the measurements a while ago, and I'm not bothered to spend the time repeating for firm numbers.

Two sets of measurements were taken: one with a load, and one with no load. The load was a 10 Ohm resistor, and the signal was 10 Hz to 20 kHz sweep.
Readings were taken with a Tektronix TBS1072 oscilloscope, using the default probes.

The resistor was inserted in series between the right channel and ground of the headphone output. The volume on the phone was increased until the waveform on the oscilloscope started to clip. The volume was backed off one step, and the peak-to-peak voltage was noted.

The resistor was removed, and the peak-to-peak voltage was again noted.

The loaded measurement was taken first, to find the clipping point / the point where the headphone output was current limited.

The voltage with the 10 Ohm resistor present was half that of no resistor case. Thus the output impedance is 10 Ohms.


Frankly this is a very poor result. Following the 1/8 rule, most headphones designed to be run by portable devices will have their sound colored according to their impedance curve.
In my case, I was using a set of Brainwavz B400. With their low impedance (30 Ohms), high sensitivity (115 dB) and multiple BA drivers, the sound from them took on a noticable treble boosted tilt.