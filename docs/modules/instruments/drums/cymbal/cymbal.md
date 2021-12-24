#abstract

a module modelling the sound of an acoustic crash/ride cymbal. it works by generating sampled noise and sending it into two pairs of a bandpass filter and resonator, as well as a set of peak filters (for modelling bell cymbals) and a compressor

#controllers

##group 1: noise settings

- base note: the base pitch of the sampled noise in semitones. 0 (80) = c5. lower values give a sample rate reduction effect
- phase: the phase (playback position) of the noise
- random phase: the amount of randomness to apply to the phase
- random pitch: the amount of random pitch to apply in semitones/256
- noise release: the release of the noise. lower values correspond to lightly tapping the cymbal, and higher values correspond to vigourously striking the cymbal

##group 2: bandpass 1 settings

- bp 1 freq: the frequency of the bandpass filter in hertz
- bp 1 resonance: the resonance (bandwidth) of the bandpass filter

##group 3: peak settings

- peak 1 freq: the frequency of the first peak in hertz
- peak 1 gain: the gain of the first peak. has a range of +/- 24 db
- peak 2 freq: the frequency of the second peak in hertz
- peak 2 gain: the gain of the second peak. has a range of +/- 24 db

##group 4: resonator 1 settings

- resonator 1 wet: the volume of the first resonator (wet) signal. 128 (4000) = -6db
- resonator 1 feedback: the feedback of the first resonator
- resonator 1 damp: the dampening (lowpass filter) of the first resonator
- resonator 1 size: the size of the first resonator
- resonator 1 seed: the random seed for the first resonator

##group 5: bandpass 1 settings

- bp 2 freq: the frequency of the bandpass filter in hertz
- bp 2 resonance: the resonance (bandwidth) of the bandpass filter

##group 6: resonator 2 settings

- resonator 2 wet: the volume of the second resonator (wet) signal. 128 (4000) = -6db
- resonator 2 feedback: the feedback of the second resonator
- resonator 2 damp: the dampening (lowpass filter) of the second resonator
- resonator 2 size: the size of the second resonator
- resonator 2 seed: the random seed for the second resonator

##group 7: compressor settings

- comp threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- comp slope: the slope (ratio) of the compressor curve in percentage. 50 (2000) = 1:2
- comp release: the release of the compressor in milliseconds
- comp makeup: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db