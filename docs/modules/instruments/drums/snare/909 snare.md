# abstract

a simple clone of the snare drum from the roland tr-909. it works simply by mixing a tone with a pitch envelope and sampled noise

for an updated and more generalized version of this module, please see my analog snare module

# controllers

## group 1: body controls

- body max tone: the tone of the body at the pitch envelope's maximum amplitude
- body min tone: the tone of the body at the pitch envelope's minimum amplitude
- body phase: the starting phase of the body. 8192 (2000) = pi/2
- body release: the release time of the body
- body volume: the volume of the body in terms of the peak level. 128 = -6db

## group 2: tail controls

- tail tone: the pitch of the sampled noise. 16384 (4000) = c5. lower values give a sample rate reduction effect
- tail phase: the phase (playback position) of the sampled noise
- body release: the release time of the tail
- body volume: the volume of the tail in terms of the peak level. 128 = -6db