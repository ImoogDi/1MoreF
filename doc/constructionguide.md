#  1MoreF
 Construction of CEM/AS3320 analog filter eurorack-modul.

**Table of Contents**

- [Preconditions](#preconditions)
- [Construction](#construction)
- [First Switchon](#firstswitchon)
- [License](#license)

## Preconditions<a name="preconditions"></a>

- All parts must be available for Board A and B (see BOM-files: [Board A](./../hw/1MoreF_BoardA_BOM.pdf) and [Board B](./../hw/1MoreF_BoardB_BOM.pdf)).
- The frontpanel is required for soldering Board A.

## Construction<a name="construction"></a>

>### Board A backside (start soldering here!) [backside-parts](./pictures/1MoreF_BoardA_parts_backside.png)

> start soldering parts on backside of Board A. **Don't solder** DIL14-socket for IC1 yet.  

>- Resistor R8 is optional and only required if **1V/octave range adjustment** is **not required**.
>- fit resistors R9, R15, R20 on backside and solder them.
>- fit multipoint connectors K7, K8 on backside and solder them.

>### Board A topside [topside-parts](./pictures/1MoreF_BoardA_parts_topside.png)

> continue soldering parts on topside of Board A.  

>- fit resistors R11, R14, R17, R21 on topside and solder them.
>- now place that DIL14-socket for IC1 on **backside** (keep mind of the right alignment).
>- solder that DIL14-socket on topside.
>- fit all remaining resistors on topside and solder them.
>- fit diode D1 on topside and solder it.
>- fit capacitor C1, C2 to topside and solder them.
>- fit capacitor C31 or C32 (depending of available type) on topside and solder it.
>- fit potentiometer P61 or P62 or P63 (dependend of available type) on topside, be carefull using spacers or some parts of PCB between the potentiometer and the soldered contacts on PCB ([spacer](./pictures/1MoreF_BoardA_spacer_under_pot.png))
>- **Don't solder yet any parts before alignment to the frontpanel**
>- fit that snapin-potentiometers P1, P2, P3, P4 and P5 on topside of PCB.
>- fit that switch S1 on topside of PCB.
>- fit that five jacks K1, K2, K3, K4 and K5 on topside of PCB.
>- place the **frontpanel** on all of the topside parts and **allign** them.
>- use nuts for the jacks, switches and pots to fix that frontpanel to the PCB-parts.
>- now solder all parts on backside and make sure everything is still alligned.
>- take a final view on Board A and place that IC: TL074 into the DIL14-socket.
>- at least Board A sould look like this: [BoardA topview](./pictures/1MoreF_BoardA_top.png)

>### Board B backside (start soldering here!) [backside-parts](./pictures/1MoreF_BoardB_parts_backside.png)

> start soldering parts on backside of Board B.  

>- fit headers K2, K3 on backside and solder them.

>### Board B topside [topside-parts](./pictures/1MoreF_BoardB_parts_topside.png)

> continue soldering parts on topside of Board B.  
> Resistors R1 ... R5 (100kOhm / 1%) **must be matched as close as possible**, only the relative value is important. Select them from that available 100k resistor-batch.

>- fit that well matched Resistors R1, R2, R3, R4 and R5 on topside and solder them.
>- fit all remaining resistors on topside and solder them.
>- fit capacitor C_11 or C_12 (depending of available type) to topside and solder it.
>- fit capacitors C_21 or C_22 and C_31 or C_32 (depending of available type) to topside and solder them.
>- fit electrolyte capacitors C3 and C4 on topside and solder them. Be carfull to **align the 'Plus'-marker** on the capacitors to the '+' on the silk.
>- fit styrene capacitors C8, C9, C10 and C11 to topside and solder them.
>- fit all remaining capacitors on topside and solder them.
>- fit the DIL18 socket X2 (for IC2) to topside and solder it.
>- fit the DIL14 socket X1 (for IC1) to topside and solder it.  
>- fit precision trimmer P_11 or P_12 (depending of available type) to topside and solder it.<br> **This is only required if 1V/octave range adjustment is required and the resistor R8 on Board A isn't soldered in.**
>- fit precision trimmer P_21 or P_22 (depending of available type) to topside and solder it.
>- fit header K1 to topside (watch correct alignment to the silk) and solder it.
>- fit the beads Filter1 and Filter2 to topside and solder them.
>- take a final view on Board B and place that IC1: TL074 into socket X1.
>- IC2: AS3320 is placed on socket X2 after the [First Switchon](#firstswitchon) -check.
>- at least Board B sould look like this (with AS3320 in socket X2): [BoardB topview](./pictures/1MoreF_BoardB_top.png)


## First Switchon<a name="firstswitchon"></a>
 Preconditions:

- IC2:=AS3320 isn't yet fitted into the socket X2 on Board B.
- Board A and B are mounted together with there header and multipoint connectors.
- The frontpanel is placed on Board A and all nuts and knobs are mounted.
- 16pin buscabel is connected between eurorack-bus and the modul (watch the alignment of Pin1 := -12V).

 Action:

- Switch on the power on the eurorack-case.
- measure the voltage on socket X2, Pin14. Must be +12Volt.
- measure the voltage on socket X2, Pin13. round about -12Volt (without current-flow).
- measure the voltage between testpoint P1 and Ground GND.

 Result:

> measured voltages on TP1 depending on the **'Frequency'**-potentiometer position.  

>Poti-position | measured voltage on TP1 (mVolt)
>--------------|---------------------------------
> min (CCW)    | less then:  +200 mVolt
> max (CW)     | higher then: -100 mVolt

> if this doesn't fit to above voltage-range the precision trimmer P_21 | P_22 (*offset*) has to be adjusted until that voltages are reached.

 Postconditions:

- IC2:=AS3320 is pushed into socket X2 on Board B.
- Calibration of the modul is required.



## License<a name="license"></a>
> Hardware:cc by-nc-sa 4.0

