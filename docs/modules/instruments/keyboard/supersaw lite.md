# abstract

a version of the analog generator with seven voices of unison with detune, blend, and random phase

along with the classic supersaw sound, you can also use this to create many more types of ~~beehives~~ unison sounds and almost anything that the analog generator is capable of doing

the difference between this and the supersaw is the detune is controlled by multisynths, which makes it use less cpu but also make it nonadjustable in real time
 
while this is superceded by my supersaw ii module, this is still maintained because the cpu load of that module may be too much for some users

# controllers

## group 1: unison settings

- detune: the detune of the voices. maximum detune means the outermost voices are detuned by one semitone
- random phase: the amount of phase randomness for each voice
- blend: the volume of the non-center voices

## group 2: waveform settings

- waveform: the waveform oscillator

## group 3: amp envelope settings

- attack: the attack of the amp envelope
- release: the release of the amp envelope
- sustain: enables the amp envelope sustain

## group 4: oscillator settings

- duty cycle: the pulsewidth (duty cycle) of the pulse waveform
- osc2 freq: the pitch of the second oscillator relative to the input pitch in semitones/64. 0 means the second oscillator is disabled

## group 5: filter settings

- filter: the type of filter or lack thereof
- f.freq: the cutoff of the filter in hertz. exponential if the "f.exponential freq" controller is enabled
- f.resonance: the resonance of the filter
- f.exponential freq: enables the exponential cutoff frequency of the filter
- f.attack: the attack of the filter envelope
- f.release: the release of the filter envelope
- f.envelope: the type of filter envelope or lack thereof

## group 6: additional settings

- monophonic: enables monophony. disabled is 4 voices polyphony
- lq: enables low-qualty oscillators
- noise: the volume of the voice white noise in terms of the peak level. 128 (4000) = -6db

## group 7: osc2 settings

- osc2 volume: the volume of the voice second oscillator in terms of the peak level. 16384 (4000) = -6db
- osc2 mode: the mix mode of the voice second oscillator