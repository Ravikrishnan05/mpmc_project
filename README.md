# mpmc_project
what is ADC?
Successive Approximation Register Analog-to-Digital Converters
//
Ldr supplies analog values when resistance changes 
The SAR ADC on MSP430 converts the analog values supplied by the LDR to digital values

# code
P1DIR |= BIT0; configures P1.0 as an output pin,
while P1DIR &= ~BIT0; configures P1.0 as an input pin.
