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

## _> Background/ Origin/ Road Map

history of product
30,000 BC-dogs were first alarms system of human race
3,000 BC -stone walls and moats
1850-Magnetic contacts were installed on entry points which on disconnecting would trigger an alarm
1990-motion detectors trigger alarms if they detect someone in an area they shouldnt be.
2010-smart iot devices allow response to any security issues with higher level of efficiency. 
in https://issuu.com/irjet/docs/irjet-v8i215

## _> Introduction
 In this era security is major issue security system is very essential these days as intrusions are increasing year after year. We should use latest technologies as thieves are also getting smarter, they now know how to break locks. We need a security system that is satisfactory in terms of security as well as cheap.LDR (Light dependent resistor) is the main component of this system as it detects the intrusion in the laser which then further sends signal to microcontroller. The second major component of this system is msp430 microcontroller which is be used to inform the owner about the intruder with an alert. This system is one of the efficient and cheapest security system that can be used anywhere not only in homes but also in farms to protect plants from animanls.
write in own words
https://issuu.com/irjet/docs/irjet-v8i215


## commercial product 
Laser-Enabled Security System Kit
$75.00
Designed for students of all ages, this kit gives students an opportunity to build their own laser-enabled security system. Equipped with a laser, photo sensor, sound alarm, and all necessary tools, this kit can be used for classroom activities and outreach events.
When using this kit, through interactive exploration and engagement, students enhance their critical thinking, problem solving, troubleshooting, and soft skills.
## working priciple



LDR's resistance varies as a function of light. The value of electrical resistance 
of a LDR is low when there is light on it (can drop to 50 ohms) and high when it is dark (several Meg ohms).
these resistances will be converted to voltages as current flows through it. 
LM393 voltage comparator compares input voltages and measures which input voltage is larger, then it provides output 
then  the analog voltages supplied by LM393 converted to digital by using ADC convertor which gives 0 with it is less than 512.
1 when it is more than 512 as input to msp430.then microcontroller gives this output as input to buzzer as 1 to alarm 0 to off.   
// just have it 
The resistance of an LDR varies inversely with the intensity of light falling on it. When there is more light, the resistance of the LDR decreases, and when there is less light, the resistance of the LDR increases. The voltage divider circuit consisting of an LDR and a fixed resistor connected in series between the power supply and ground can be used to convert the resistance of the LDR to a voltage. The output voltage is proportional to the resistance of the LDR. The LM393 voltage comparator compares the input voltages and provides output based on which input voltage is larger. The analog voltages supplied by LM393 are converted to digital using an ADC converter. If the output of ADC is less than 512, it gives 0, and if it is more than 512, it gives 1 as input to MSP430 microcontroller. The microcontroller then gives this output as input to a buzzer as 1 to alarm and 0 to turn off.
## novelty 

We are the first ones to do laser security system with msp430 microcontroller and ldr with LM393 voltage comparator.
MSP430 is known for its extremely low power consumption when compared to other microcontrollers, which makes it suitable for energy-efficient application
in our project case.
this makes our project unique.

## future enhancement 
* we can make it as laser fencing used by indian army on further enhancement 
*protecting crops by scaring the animals through alarm
sound that is obtained through laser beam interruption caused by intruding animals.
## > Literature (ACS/ Nature/ Wiley/ IEEE Journals)

> https://www.ijser.org/researchpaper/LASER-SECURITY-SYSTEM-Suman.pdf
> https://www.irjet.net/archives/V5/i1/IRJET-V5I1163.pdf
> https://www.iaps.org.in/journal/index.php/journaliaps/article/view/133
> https://www.drdo.gov.in/laser-fencing
