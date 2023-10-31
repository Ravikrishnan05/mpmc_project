# mpmc_project
what is ADC?
Successive Approximation Register Analog-to-Digital Converters
//
Ldr supplies analog values when resistance changes 
The SAR ADC on MSP430 converts the analog values supplied by the LDR to digital values
# connections 
For ldr 
vcc-5v in msp
ground
do-digital output to any pin from 1.0 to 1.7 but while change this[P1DIR &= ~BIT0] as required;

For buzzer 
one end to ground another end to p[1.0-1.7]
another end to ground in msp430

# code
P1DIR |= BIT0; configures P1.0 as an output pin,
while P1DIR &= ~BIT0; configures P1.0 as an input pin.

# presentation

_> Background/ Origin/ Road Map

history of product
30,000 BC-dogs were first alarms system of human race
3,000 BC -stone walls and moats
1850-Magnetic contacts were installed on entry points which on disconnecting would trigger an alarm
1990-motion detectors trigger alarms if they detect someone in an area they shouldnt be.
2010-smart iot devices allow response to any security issues with higher level of efficiency. 
in https://issuu.com/irjet/docs/irjet-v8i215

_> Introduction

write in own words
https://issuu.com/irjet/docs/irjet-v8i215

> Literature (ACS/ Nature/ Wiley/ IEEE Journals)
> https://www.ijser.org/researchpaper/LASER-SECURITY-SYSTEM-Suman.pdf
> https://www.irjet.net/archives/V5/i1/IRJET-V5I1163.pdf


