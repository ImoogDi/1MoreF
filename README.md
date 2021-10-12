#  1MoreF
> Eurorack filter based on CEM/AS3320 used in modular Synthesizers.

**Table of Contents**

- [Introduction](#intro)
- [Construction Guide](./doc/constructionguide.md)
- [Calibration](./doc/calibration.md)
- [Technical data](#technical-data)
- [License](#license)

## Introduction<a name="intro"></a>

This eurorack-modul is designed for modular-synthesizers as substractive filter.  
The filter is build around that IC: AS3320, a clone of that old CEM3320.  
All parts are common available and DIY-friendly designed.

- Modul Frontpanel

![Modul: 1MoreF Front](./doc/pictures/1MoreF_Modul.png)

- Modul Backside

![Modul: 1MoreF Backside](./doc/pictures/1MoreF_ModulBackKomlete.png)

There are five 3.5mm jacks available for patching audio- and CV-signals.  

Jack-Name | Function                       | Comment
----------|--------------------------------|-----------------------------------
IN        | audio-input                    | Level adjustable between 0 ...  2  
ResCV     | CV-input for resonance control | Level adjustable between 0 ... 10  
          |                                | (only positiv voltage is used,  
          |                                |  negativ voltages are clipped)  
Mod.      | CV-input for modulation control| Level adjustable between -  0  +  
OUT       | audio-output for HP/LP/BP mode | audio-output attached to switch  
          | (12dB/octave)                  |  HP := High pass mode  
          |                                |  LP := Low pass mode  
          |                                |  BP := Band pass mode  
LP24      | audio-output for LP mode only  | Low pass only audio-output with  
          | (24dB/octave)                  | 24dB/octave  
          |                                | (simultaneously usable with 'OUT')  
          |                                |

There are six potentiometers with following functions:  

Poti-Name | Function                       | Comment
----------|--------------------------------|-----------------------------------
Frequency | Cut-Off frequency 20Hz to 20kHz| Filter cutoff frequency, range:  
          |                                | min := < 20 Hz  
          |                                | max := > 20kHz  
          |                                | 12 o'clock position := 440Hz  
Track     | Keyboard-CV tracking potentiom.| Keyboard-CV tracking adjustable  
          |                                |  0 := None  
          |                                |  1 := 1V/octave  
Res.      | Resonance potentiometer        | Resonance adjustment  
          |                                |  0 := None  
          |                                | 10 := maximum, self oscillation  
          |                                | 12 o'clock position := starting oscillation  
IN        | Audio input-level attenuator   | Level adjustable between 0 ... 2  
          |                                |  0 := No audio signal from IN-jack  
          |                                |  1 := audio signal OUT-level is 1 * IN-level  
          |                                |  2 := audio signal OUT-level is 2 * IN-level  
ResCV     | Resonance-CV attenuator        | Resonance-CV attenuator  
          |                                |  0 := None  
          |                                | 10 := maximum  
Mod.      | Modulation-CV attenuverter     | Modulation-CV attenuverter, controlling  
          |                                | the amount and polarity of modulation  
          |                                |  - := negative modulation  
          |                                |  + := positive modulation  
          |                                |  0 := no modulation  
          |                                |


## Technical data<a name="technical-data"></a>

- size:  
  width: 8HP  
  depth: 40mm

- power:  
    5Volt, 0 mA  
  +12Volt, 25mA  
  -12Volt, 25mA  

- frequency range: 20Hz to 20kHz.
- frequency CV scale: 1V/Oct.
- signal input, AC-coupled signal path.
- modulation inputs, DC-coupled signal path.
- signal input impedance: > 50kOhm.
- signal output impedance: 470 Ohm.
- CV-Input impedance: 100kOhm.


## License<a name="license"></a>
> Hardware:cc by-nc-sa 4.0

