#abstract

a clone of the exciter effect from the calf plugin suite

it is essentially a mid-band saturator. it splits the audio into three bands and saturates the mid band

use it to make your sounds more crispy

unlike the original effect, this module uses inversion-based splitting to negate phase coloration

the waveshaper curves were generated using pixilang, i'll see if i can find the original file

#controllers

##group 1: split controls

- scope: the frequency of the band 1/2 split in hertz
- ceiling: the frequency of the band 2/3 split in hertz

##group 2: saturator controls

- input gain: the input gain of the signal in terms of the peak value. 256 (2000) = 0db
- odd/even harmonics: the mix of the symmetrical/asymmetrical saturators
- character: the curve shape of the saturator
- mix: the dry/wet mix of the saturation. 16384 (4000) = 50% dry 50% wet