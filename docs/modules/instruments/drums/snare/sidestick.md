# abstract

a module simulating the sound of an acoustic snare drum when played using the sidestick technique. it works by generating doubly triggered filtered sampled noise and sending it to a head and body resonator

this module used to be called "rim", but i changed it after i learned that this term is erroneous

# controllers

## group 1: noise main settings

- base note: the base pitch of the sampled noise in semitones. 0 (80) = c5. lower values give a sample rate reduction effect
- noise phase: the phase (playback position) of the noise
- noise random pitch: the amount of random pitch to apply in semitones/256
- noise random phase: the amount of randomness to apply to the phase

## group 2: rehit settings

- rehit delay: the delay for the retrigger in the chosen unit
- rehit delay unit: the unit for the retrigger delay

## group 3: noise misc settings

- noise release: the release time for the noise
- noise resonance: the resonance for the 12db bandpass filter

## group 4: head resonator settings

- head resonate amount: the volume of the resonator (wet) signal in terms of the peak level. 128 (4000) = -6db
- head resonate ring: the feedback of the head resonator
- head resonate tension: the dampening (lowpass filter) of the head resonator
- head resonate size: the size of the head resonator
- head resonate seed: the random seed of the head resonator

## group 5: body resonator settings

- body resonate amount: the volume of the resonator (wet) signal in terms of the peak level. 128 (4000) = -6db
- body resonate ring: the feedback of the body resonator
- body resonate tension: the dampening (lowpass filter) of the body resonator
- body resonate size: the size of the body resonator
- body resonate seed: the random seed of the body resonator