# abstract

a module modelling the sound of an acoustic snare drum. it works by generating four sine waves with random frequencies and amplitudes as the head of the snare. the head is sent to a head resonator, and then a body resonator. there are also two sampled noise oscillators simulating the snares and the stick, both of which are filtered and sent to the body resonator

# controllers

## group 1: overall settings

- all transpose: the base pitch of all the sounds in semitones. 0 (80) = c5

## group 2: snares settings

- snares transpose: the pitch of the sampled noise relative to the base pitch. 0 (80) = base pitch. lower values give a sample rate reduction effect
- snares random pitch: the amount of random pitch to apply in semitones/256
- snares phase: the phase (playback position) of the sampled noise
- snares random phase: the amount of randomness to apply to the phase
- snares volume: the volume of the sampled noise. 16384 (4000) = -6db
- snares ringiness: the resonance of the pitchtracked bandpass filter on the sampled noise
- snares min amp release: the release of the noise amplitude envelope at minimum velocity
- snares max amp release: the release of the noise amplitude envelope at maximum velocity
- snares min filter release: the release of the noise filter envelope at minimum velocity
- snares max filter release: the release of the noise filter envelope at maximum velocity

## group 3: head settings

- head transpose: the pitch of the head relative to the base pitch. 0 (80) = base pitch.
- head volume: the volume of the head. 16384 (4000) = -6db
- head release: the release of the amplitude envelope.
- head harmonics: the amount (gain) of harmonics besides the fundamental. 32768 (8000) makes the harmonics at equal volume with the fundamental (you may want to turn down the head volume to compensate)
- head harmonic frequency distribution: the random seed for the harmonic frequency distribution. note that while there are 256 distinct seeds, they are also interpolated, so you can get variations on the current seed +/-128 units from the current seed
- head harmonic amplitude distribution: the random seed for the harmonic amplitude distribution. note that while there are 256 distinct seeds, they are also interpolated, so you can get variations on the current seed +/-128 units from the current seed

## group 4: head resonator settings

- head ringiness: the feedback of the head resonator
- head tension: the dampening (lowpass filter) of the head resonator
- head size: the size of the head resonator
- head seed: the random seed of the head resonator

## group 5: body settings

- body min wet: the amount of resonated (wet) signal at minimum velocity. 16384 (4000) = -6db
- body max wet: the amount of resonated (wet) signal at maximum velocity. 16384 (4000) = -6db
- body ringiness: the feedback of the body resonator
- body tension: the dampening (lowpass filter) of the body resonator
- body size: the size of the body resonator
- body seed: the random seed of the body resonator