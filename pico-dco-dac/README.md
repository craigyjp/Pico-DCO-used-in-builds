# Raspberry Pi Pico Polyphonic DCO

This board was modified from the original Pico DCO to act as a secondary DCO board to provide 2 DCO's per voice, as the first DCO board has gate outputs these were not deemed necessary on the second DCO board. This board does not have a MIDI input and takes its MIDI signal from the first board via a buffer, stacking controls are also shared between the 2 boards. Detune and FM inputs are currently seperate, but I think the FM inputs can be linked.

This repository contains source code, schematics for a digitally controlled oscillator (DCO) with up to 6 voices which are driven by a Raspberry Pi Pico. It uses PIO to generate a highly accurate frequency which is controlled by USB or serial MIDI. The analog oscillator part is based on the Juno 106 and generates sawtooth and square wave signal with a 10Vpp amplitude. Amplitude compensation is done by a smoothed PWM signal coming from the Pico. Additionally I have removed the gate signals and added 2x 8 channel DACs to provide the 6 CV's and 6 velocity CV's that would normally be available for filter tracking, levels etc. This also makes the board into a 6 note polyphonic MIDI to CV converter. Additionally with the help of Freddie Renyard an FM input is now available. Also an octave select switch allowing a 3 octave adjustment of the DCO's range.

## Key features

- Digitally controlled analog oscillator using a Raspberry Pi Pico
- Up to six voices
- Voice stacking
- Detuning of voices
- 2x 8 channel DAC (DAC8568) for CV and velocity
- DIN MIDI serial input
- USB MIDI input
- MIDI pitch bend
- Portamento with adjustable speed
