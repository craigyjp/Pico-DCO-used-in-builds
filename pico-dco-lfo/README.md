# Raspberry Pi Pico Polyphonic DCO

This repository contains source code, schematics and PCB for a digitally controlled oscillator (DCO) with up to 6 voices which are driven by a Raspberry Pi Pico. It uses PIO to generate a highly accurate frequency which is controlled by USB or serial MIDI. The analog oscillator part is based on the Juno 106 and generates sawtooth and square wave signal with a 10Vpp amplitude. Amplitude compensation is done by a smoothed PWM signal coming from the Pico.

## Key features

- Digitally controlled analog oscillator using a Raspberry Pi Pico
- Up to six voices
- Voice stacking
- Detuning of voices
- Separate gate signal
- DIN MIDI serial input
- USB MIDI input
- MIDI pitch bend
- Portamento with adjustable speed
- FM input
