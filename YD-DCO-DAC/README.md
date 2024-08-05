# Raspberry Pi Pico Polyphonic DCO

This repository contains source code, schematics and PCB for a digitally controlled oscillator (DCO) with up to 8 voices which are driven by a Raspberry Pi Pico. It uses PIO to generate a highly accurate frequency which is controlled by USB or serial MIDI. The analog oscillator part is based on the Juno 106 and generates sawtooth and square wave signal with a 10Vpp amplitude. Amplitude compensation is done by a smoothed PWM signal coming from the Pico.

# Used in the PolyKit-16 in a 3 way config, 2 pico-dco-lfo and 1 pico-dco-dac, second lfo was set to midi channel 2

## Key features

- 8 gate ouputs
- 2x 8 channel DAC (DAC8568) for CV and velocity
- DIN MIDI serial input
- USB MIDI input

