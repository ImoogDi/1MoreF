#  1MoreF
> Calibration of CEM/AS3320 analog filter eurorack-modul.

## Preconditions<a name="preconditions"></a>
 Required or recommended tools are:

- 440Hz tone-reference (tuning-fork, fork oscillator etc.).
- Voltage meter.
- Resistance meter.
- Frequency meter (if available).
- Eurorack for power (+12V/-12V) and keyboard-CV.
- 16pin Eurorack cable for modul-connection to the rack-bus.
- patchcables for modular synthesizers.

## Calibration<a name="calibration"></a>

**Table of Contents**

- [Offset-Adjustment](#offset_adjustment)
- [1V/Oct.-Adjustment](#1V_oct_adjustment)
- [Final check](#final_check)
- [License](#license)

### Offset-Adjustment<a name="offset_adjustment"></a>
 Offset-adjustment is done with potentiometer 'P2' on board B.  
>- Set **'Frequency'**-potentiometer to 12 o'clock position.  
>- Set **'Res.'** (resonance)-potentiometer to value:10 (**'CW'**, self oscillating).  
>- Set **'Mod'** (modulation)-potentiometer to 12 o'clock position (0 := no modulation).  
>- Set **all other** potentiometers to **CCW** position.  
>- connect 16pin eurorack cable from rack-bus to the socket Pin1 on board B. Be **carefull** to fit the allignment of buspower Pin1 (-12V) .  
>- connect patchcable between signal-output **'OUT'** and audio-out (or frequency meter, if available).  
>- power up the eurorack.  
>- Turn precision trimmer **'P2' on 1MoreF board B** until the soundable- or measured- frequency is close as possible to 440Hz.

### 1V/Oct.-Adjustment<a name="1V_oct_adjustment"></a>
 The CV-range (1V/octave) must be tuned with potentiometer 'P1' on board B after the offset-adjustment .  
 The **'Res.'** (resonance)-potentiometer must be set to value:10 (**'CW'**, self oscillating).  
>- Set the keyboard-CV for playing key-note **A4**.  
>- Set **'Track'**-potentiometer to full **CW**.  
>- Turn **'Frequency'**-potentiometer **CCW** until the soundable- or measured- frequency is again 440Hz.  
>- play key-note **A3** and check the measured frequency. If the measurement is above 220Hz, then turn 'P1'-potentiometer **'CCW'**, else **'CW'**.  
>- play key-note **A5** and check the measured frequency. If the measurement is above 880Hz, then turn 'P1'-potentiometer **'CCW'**, else **'CW'**.

 Repeat this adjustment until the measuared frequencies are A2=110Hz, A3=220Hz, A4=440Hz and A5=880Hz.  
 Repeat also the 'offset-adjustment to fit the 440Hz to 12 o'clock position on **'Frequency'**-potentiometer.  

### Final check<a name="final_check"></a>
 Voltage measurement on Testpoint: TP1.  

 The **'Res.'** (resonance)-potentiometer must be set to value:10 (**'CW'**, self oscillating).  
 Set **all other** potentiometers to **CCW** position.  
 >- connect voltage-meter between GND and TP1.  

 The following table shows the measured voltages depending on the **'Frequency'**-potentiometer position.  

Poti-position | Frequency (Hz)       | measured voltage on TP1 (mVolt)
--------------|----------------------|-----------------------------------
 min (CCW)    | less then 20 Hz      | 175 mVolt
 12 o'clock   | 440 Hz               |  84 mVolt
 max (CW)     | above 20 kHz         | -47 mVolt


## License<a name="license"></a>
> Hardware:cc by-nc-sa 4.0

