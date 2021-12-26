# abstract

a module simulating the sound of an acoustic grand piano. thanks to logickin for some help and suggestions

it works via hybrid subtractive/physical modelling synthesis, where for each voice, two detuned pulse waves are sent to two parallel comb filters operating as waveguides. then, all three signals are sent to a 48db enveloped lowpass filter, then an amplitude modulator with an envelope

each voice is then sent to a set of soundboard and body resonators, then a high shelf and high pass filter for sound adjustment

the module has ten voices of polyphony and uses cyclic round-robin voice allocation

the module responds to velocity, so lower velocities mean less harmonics

the module sounds great with some reverb, preferably my reverb pro module

the module was called "sunforte" in reference to the piano's original name, the pianoforte, though perhaps just "piano" would be clearer



# controllers

## group 1: pedals

- sustain pedal: enables the sustain pedal

## group 2: physical modelling settings

- soundboard seed: the random seed for the soundboard resonator
- body seed: the random seed for the body resonator
- key strike volume: the volume of the key strike sound in terms of the peak level. 16384 (4000) = -6db
- hammer position: the pulsewidth (duty cycle) of the oscillators, simulating the position of the hammers

## group 3: waveguide settings

- waveguide 1 delay: the delay of the first waveguide. has a maximum delay of one second
- waveguide 2 delay: the delay of the second waveguide. has a maximum delay of one second
- waveguide 1 feedback: the feedback of the first waveguide
- waveguide 2 feedback: the feedback of the second waveguide

## group 4: other settings

- beating amp: the volume of the second oscillator in terms of the peak level. 16384 (4000) = -6db. this changes the amount of beating (frequency interference) in the sound

## group 5: tone control

- highs gain: the gain of the high shelf filter. set to 4006 hertz
- lows cut: the frequency of the 12db highpass filter in hertz

## group 6: sound2ctl sample rate settings

- filter envelope sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot
