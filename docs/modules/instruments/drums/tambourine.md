#abstract

a module modelling the sound of an acoustic tambourine. it works by sending sampled noise into a set of parallel bandpass filters and then a resonator

#controllers

##group 1: noise main settings

- noise transpose: the base pitch of the sampled noise in semitones. 0 (80) = c5. lower values give a sample rate reduction effect
- noise random pitch: the amount of random pitch to apply in semitones/256
- noise phase: the phase (playback position) of the noise
- noise random phase: the amount of randomness to apply to the phase
- noise volume: the volume of the sampled noise. 128 (4000) = -6db
- noise release: the release of the noise

##group 2: noise initital filter

- noise filter freq: the frequency of the noise 12db highpass filter in hertz
- noise filter resonance: the resonance of the noise 12db highpass filter

##group 3: bandpass filter bank settings

- bandpass 1 freq: the frequency of the first bandpass filter in hertz
- bandpass 1 resonance: the resonance (bandwidth) of the first bandpass filter
- bandpass 2 freq: the frequency of the second bandpass filter in hertz
- bandpass 2 resonance: the resonance (bandwidth) of the second bandpass filter
- bandpass 3 freq: the frequency of the third bandpass filter in hertz
- bandpass 3 resonance: the resonance (bandwidth) of the third bandpass filter
- bandpass 4 freq: the frequency of the fourth bandpass filter in hertz
- bandpass 4 resonance: the resonance (bandwidth) of the fourth bandpass filter

##group 4: resonator settings

- resonator wet: the amount of resonated (wet) signal. 128 (4000) = -6db
- resonator feedback: the feedback of the resonator
- resonator damp: the dampening (lowpass filter) of the resonator
- resonator size: the size of the resonator
- resonator seed: the random seed of the resonator