# abstract

a clone of lmms's triple oscillator plugin, minus some controls and modulation types

this is the monophonic version, which uses eight times less cpu than the polyphonic version

note that the envelope affects the output sound and not the individual oscillators

# controllers

## group 1: adsr settings

- attack: the attack of the adsr amp envelope
- decay: the decay of the adsr amp envelope
- sustain level: the sustain level of the adsr envelope
- release: the release of the adsr amp envelope

## group 2: osc 1 settings

- osc 1 volume: the volume of oscillator 1 in terms of the peak level. 16384 (4000) = -6db
- osc 1 panning: the panning of oscillator 1
- osc 1 waveform: the waveform of oscillator 1
- osc 1 coarse: the coarse detune from the input pitch of oscillator 1 in semitones
- osc 1 fine: the fine detune from the input pitch of oscillator 1 in semitones/256
- osc 1 phase: the phase of oscillator 1. 8192 (2000) = pi/2

## group 3: osc 2 settings

- osc 2 volume: the volume of oscillator 2 in terms of the peak level. 16384 (4000) = -6db
- osc 2 panning: the panning of oscillator 2
- osc 2 waveform: the waveform of oscillator 2
- osc 2 coarse: the coarse detune from the input pitch of oscillator 2 in semitones
- osc 2 fine: the fine detune from the input pitch of oscillator 2 in semitones/256
- osc 2 phase: the phase of oscillator 2. 8192 (2000) = pi/2

## group 4: osc 3 settings

- osc 3 volume: the volume of oscillator 3 in terms of the peak level. 16384 (4000) = -6db
- osc 3 panning: the panning of oscillator 3
- osc 3 waveform: the waveform of oscillator 3
- osc 3 coarse: the coarse detune from the input pitch of oscillator 3 in semitones
- osc 3 fine: the fine detune from the input pitch of oscillator 3 in semitones/256
- osc 3 phase: the phase of oscillator 3. 8192 (2000) = pi/2

## group 5: modulation settings

- osc 1 -> osc 2 mod enable: enables modulation between oscillators 1 and 2
- osc 1 -> osc 2 mod rm/pm: switches between ring modulation and phase modulation between oscillators 1 and 2
- osc 2 -> osc 3 mod enable: enables modulation between oscillators 2 and 3
- osc 2 -> osc 3 mod rm/pm: switches between ring modulation and phase modulation between oscillators 2 and 3

## group 6: additional settings

- lq: enables low-quality mode for the oscillators