# abstract

a module modelling the sound of an acoustic shaker. it works simply by sending filtered sampled noise to a resonator and a second filter

# controllers

## group 1: noise controls

- base note: the base pitch of the sampled noise in semitones. 0 (80) = c5. lower values give a sample rate reduction effect
- noise phase: the phase (playback position) of the noise
- random pitch: the amount of random pitch to apply in semitones/256
- random phase: the amount of randomness to apply to the phase

## group 2: envelope controls

- noise attack: the attack of the noise envelope
- noise release: the release of the noise envelope

## group 3: noise filter controls

- noise filter: the type of filter to apply to the noise
- noise filter frequency: the frequency of the noise filter in hertz. this is exponential when the "noise filter exponential" controller is on
- noise filter resonance: the resonance of the noise filter
- noise filter exponential: enables the exponential frequency mode for the filter

## group 4: resonator controls

- resonate wet: the volume of the resonator (wet) signal. 128 (4000) = -6db
- resonate feedback: the feedback of the resonator
- resonate damp: the dampening (lowpass filter) of the resonator
- resonate size: the size of the resonator
- resonate seed: the random seed for the resonator

## group 5: postfilter controls

- filter frequency: the frequency of the filter in hertz
- filter resonance: the resonance of the filter
- filter type: the type of filter to use