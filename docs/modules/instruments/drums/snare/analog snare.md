# abstract

a module simulating the snare sound produced by many analog drum machines. it works simply by generating a low tone with a pitch envelope and some mild saturation, as well as sampled noise with an amplitude envelope

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

# controllers

## group 1: body settings

- body amt: the volume of the body in terms of the peak value. 16384 (4000) = -6db
- body coarse: the coarse pitch of the body in semitones. 0 (80) = c5
- body fine: the fine pitch of the body in semitones/256.
- body phase: the starting phase of the body. 8192 (2000) = pi/2
- body release: the release time of the body

## group 2: pitch env controls

- pitch env amt: the amount of the pitch envelope. 0 = no pitch envelope
- pitch env release: the release of the pitch envelope

## group 3: noise controls

- noise amt: the volume of the noise in terms of the peak value. 16384 (4000) = -6db
- noise phase: the phase (playback position) of the noise
- noise release: the release time of the noise
- noise filter freq: the filter frequency of the 24db highpass filter in hertz
- noise filter resonance: the filter resonance of the 24db highpass filter

## group 4: saturation controls

- sat input volume: the input gain to the saturator. note that 0 = silence