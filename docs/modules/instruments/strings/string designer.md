# abstract

a module simulating the sound of an acoustic string instument, either bowed (arco) or plucked (pizzicato). forked from philip bergwerf's module of the same name

it works via hybrid subtractive/physical modelling synthesis, where for each string, either an arco or pizzicato unit is used 

for arco, a sustained sawtooth wave is randomly frequency modulated (and non-randomly modulated for vibrato) by a set of lfos set to different frequencies. the sawtooth is sent to a velocity-controled 12db lowpass filter, then a noise ring modulator to simulate surface noise, then a sine ring modulator for tremolo, and lastly a velocity-controlled adsr modulator

for pizzicato, a sawtooth wave with a short release is sent to an adsr modulator, a 48db lowpass envelope filter, and lastly a mild sine amplitude modulator

both types are then sent into a string and body resonator

this module is velocity-enabled, and lower velocities give less harmonics

this module can create contrabass, cello, viola, and violin sounds, as well as sounds outside the ranges of these instruments

be sure to automate the parameters for more realistic articulation :>

as of 2.0, this module uses fifo-based voice allocation

# controllers

## group 1: sound selection

- arco/pizzicato: selects between arco and pizzicato playing

## group 2: arco main settings

- arco portamento amount: the amount of portamento in arco playing

## group 3: arco amplitude envelope settings

- arco amp attack: the attack of the arco amplitude envelope
- arco amp decay: the decay of the arco amplitude envelope
- arco amp sustain: enables the arco amplitude envelope sustain
- arco amp sustain level: the sustain level of the arco amplitude envelope
- arco amp release: the release of the arco amplitude envelope

## group 4: arco vibrato settings

- arco vibrato amount: the amount of the arco vibrato
- arco vibrato speed: the speed of the arco vibrato
- arco vibrato attack: the attack of the arco vibrato envelope
- arco vibrato release: the release of the arco vibrato envelope

## group 5: arco tremolo settings

- arco tremolo amount: the amount of the arco tremolo
- arco tremolo speed: the speed of the arco tremolo
- arco tremolo attack: the attack of the arco tremolo envelope
- arco tremolo release: the release of the arco tremolo envelope

## group 6: arco additonal settings

- arco random vibrato amount: the amount of arco random vibrato. a little bit makes the sound much more realistic
- arco surface noise: the amount of arco surface noise. although any string player can tell you surface noise is undesirable in most cases, i included it anyway because i wanted to simulate avant-garde playing

## group 7: physical settings

- string seed: the random seed for the string resonator
- body seed: the random seed for the body resonator