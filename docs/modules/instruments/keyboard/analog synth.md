#abstract

a monophonic analog-style synthesizer module inspired by the arp 2600, moog minimoog and others

it uses two oscillators and a noise generator mixed and sent to an adsr envelope filter, an adsr amplitude modulator, and a reverb

though the noise generator is intended to generate noise, it is also keytracked and can be used as a third oscillator

though this was succeeded my analog synth ii module, it is not obsolete; they coexist

#controllers

##group 1: osc 1 settings

- osc 1 transpose: the coarse detune of oscillator 1 in semitones
- osc 1 finetune: the fine detune of oscillator 1 in semitones/256
- osc 1 waveform: the waveform of oscillator 1
- osc 1 duty cycle: the pulsewidth (duty cycle) of oscillator 1 in the case of the pulse wave

##group 2: osc 2 settings

- osc 2 transpose: the coarse detune of oscillator 2 in semitones
- osc 2 finetune: the fine detune of oscillator 2 in semitones/256
- osc 2 waveform: the waveform of oscillator 2
- osc 2 duty cycle: the pulsewidth (duty cycle) of oscillator 2 in the case of the pulse wave

##group 3: noise settings

- noise type: the noise type/waveform of the noise generator

##group 4: filter settings

- filter freq: the exponential frequency of the filter
- filter q: the resonance of the filter
- filter type: the type of filter to use
- filter roll-off: the roll-off of thee filter in db/oct

##group 5: amp envelope settings

- amp attack: the attack of the amp envelope in milliseconds
- amp decay: the decay of the amp envelope in milliseconds
- amp sustain: the sustain mode of the amp envelope
- amp sustain level: the sustain level of the amp envelope
- amp release: the release of the amp envelope in milliseconds

##group 6: filter envelope settings

- filter attack: the attack of the filter envelope in milliseconds
- filter decay: the decay of the filter envelope in milliseconds
- filter sustain: the sustain mode of the filter envelope
- filter sustain level: the sustain level of the filter envelope
- filter release: the release of the filter envelope in milliseconds

##group 7: oscillator mix settings

- osc 1 mix: the volume of oscillator 1, in terms of the peak level. 16384 (4000) = -6db
- osc 2 mix: the volume of oscillator 2, in terms of the peak level. 16384 (4000) = -6db
- noise mix: the volume of the noise generator, in terms of the peak level. 16384 (4000) = -6db

##group 8: reverb settings

- reverb wet: the amount (wet) of the reverb. 128 (4000) = -6db
- reverb size: the size of the reverb

 