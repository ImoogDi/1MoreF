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

<table>
<tr>
    <th>Jack-Name</th>
    <th>Function</th>
    <th>Comment</th>
</tr>
<tr>
    <td>IN</td>
    <td>audio-input</td>
    <td>Level adjustable between 0 ...  2</td>
</tr>
<tr>
    <td>ResCV</td>
    <td>CV-input for resonance control</td>
    <td>Level adjustable between 0 ... 10<br>(only positiv voltages are used,<br>negativ voltages are clipped)</td>
</tr>
<tr>
    <td>Mod.</td>
    <td>CV-input for modulation control</td>
    <td>Level adjustable between -  0  +</td>
</tr>
<tr>
    <td>OUT</td>
    <td>audio-output for HP/LP/BP mode<br>(12dB/octave)</td>
    <td>audio-output attached to switch<br> HP := High pass mode<br> LP := Low pass mode<br> BP := Band pass mode</td>
</tr>
<tr>
    <td>LP24</td>
    <td>audio-output for LP mode only<br>(24dB/octave)</td>
    <td>Low pass only audio-output with<br>24dB/octave<br>(simultaneously usable with 'OUT')</td>
</tr>
</table>


There are six potentiometers with following functions:  

<table>
<tr>
    <th>Poti-Name</th>
    <th>Function</th>
    <th>Comment</th>
</tr>
<tr>
    <td>Frequency</td>
    <td>Cut-Off frequency 20Hz to 20kHz</td>
    <td>Filter cutoff frequency, range:<br>min := &#60; 20 Hz<br>max := > 20kHz<br>12 o'clock position := 440Hz</td>
</tr>
<tr>
    <td>Track</td>
    <td>Keyboard-CV tracking potentiom.</td>
    <td>Keyboard-CV tracking adjustable<br>0 := None<br>1 := 1V/octave</td>
</tr>
<tr>
    <td>Res.</td>
    <td>Resonance potentiometer</td>
    <td>Resonance adjustment<br>0 := None<br>10 := maximum, self oscillation<br>12 o'clock position := starting oscillation</td>
</tr>
<tr>
    <td>IN</td>
    <td>Audio input-level attenuator</td>
    <td>Level adjustable between 0 ... 2<br>0 := No audio signal from IN-jack<br>1 := audio signal Out-level is 1 * IN-level<br>2 := audio signal Out-level is 2 * IN-level</td>
</tr>
<tr>
    <td>ResCV</td>
    <td>Resonance-CV attenuator</td>
    <td>Resonance-CV attenuator<br>0 := None<br>10 := maximum</td>
</tr>
<tr>
    <td>Mod.</td>
    <td>Modulation-CV attenuverter</td>
    <td>Modulation-CV attenuverter, controlling<br>the amount and polarity of modulation<br>- := negative modulation<br>+ := positive modulation<br>0 := no modulation</td>
</tr>
</table>


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

