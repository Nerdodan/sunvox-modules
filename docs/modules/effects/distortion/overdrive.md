#abstract

an overdrive (distortion) effect inspired by the saturator effect from the calf plugin suite

applies heavy distortion to the signal, with optional pre- and post-filtering and tone control

use it for a wide variety of overdrive effects, including guitar distortion pedal effects

the waveshaper curves were generated using pixilang, i'll see if i can find the original file

#controllers

##group 1: main controls

- input gain: the input gain of the signal in terms of the peak value. 256 (2000) = 0db
- odd/even harmonics: the mix of the symmetrical/asymmetrical distortions
- hardness: adjusts the shape of the distortion curve. 0 = full soft clipping and 32768 (8000) = full hard clipping
- mix: the dry/wet mix of the distortion. 16384 (4000) = 50% dry 50% wet

##group 2: prefiltering

- prefilter: enables prefiltering
- pre lp: the frequency of the 12db lowpass filter in hertz
- pre hp: the frequency of the 12db highpass filter in hertz

##group 3: tone control

- tone freq: the frequency of the peak in hertz
- tone q: the resonance (bandwidth) of the peak. 0 = the peak covers the entire spectrum, use this trick to get even higher input gain
- tone gain: the gain of the peak. 16384 (4000) = 0db, 32768 (8000) = +24db

##group 4: postfiltering

- postfilter: enables postfiltering
- post lp: the frequency of the 12db lowpass filter in hertz
- post hp: the frequency of the 12db highpass filter in hertz
