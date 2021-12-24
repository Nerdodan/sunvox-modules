#abstract

a module modelling the sound of an acoustic bass drum (kick). it works by generating a mildly saturated tone with a pitch envelope, sending it into a head resonator, and sending the head resonator output into a body resonator. there is also pitchtracked bandpass filtered sampled noise simulating the lever and drum being sent directly into the body resonator

#controllers

##group 1: overall settings

- all transpose: the base pitch of all the sounds in semitones. 0 (80) = c5

##group 2: noise settings

- noise transpose: the pitch of the sampled noise relative to the base pitch. 0 (80) = base pitch. lower values give a sample rate reduction effect
- noise random pitch: the amount of random pitch to apply in semitones/256
- noise phase: the phase (playback position) of the sampled noise
- noise random phase: the amount of randomness to apply to the phase
- noise volume: the volume of the sampled noise. 128 (4000) = -6db
- noise ringiness: the resonance of the pitchtracked bandpass filter on the sampled noise
- noise min release: the release of the noise at minimum velocity
- noise max release: the release of the noise at maximum velocity

##group 3: head settings

- head transpose: the pitch of the tone relative to the base pitch. 0 (80) = base pitch.
- head volume: the volume of the tone. 128 (4000) = -6db. note that this is before the saturation
- head release: the release of the amplitude and pitch envelope in seconds/256. maximum value is 2 seconds
- head ringiness: the feedback of the head resonator
- head tension: the dampening (lowpass filter) of the head resonator
- head size: the size of the head resonator
- head seed: the random seed of the head resonator

##group 4: body settings

- body min wet: the amount of resonated (wet) signal at minimum velocity. 16384 (4000) = -6db
- body max wet: the amount of resonated (wet) signal at maximum velocity. 16384 (4000) = -6db
- body ringiness: the feedback of the body resonator
- body tension: the dampening (lowpass filter) of the body resonator
- body size: the size of the body resonator
- body seed: the random seed of the body resonator