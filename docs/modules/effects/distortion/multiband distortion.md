# abstract

a four-band variant of the stock distortion module

distorts each band separately and sums the bands

uses inversion-based band splits to negate phase coloration

# controllers

## group 1: band split

- band 1/2 split: the split frequency of bands 1 and 2 in hertz
- band 2/3 split: the split frequency of bands 2 and 3 in hertz
- band 3/4 split: the split frequency of bands 3 and 4 in hertz

## group 2: input gain control

- band 1 input gain: the input gain of band 1 in terms of the peak value. 256 (2000) = 0db
- band 2 input gain: the input gain of band 2 in terms of the peak value. 256 (2000) = 0db
- band 3 input gain: the input gain of band 3 in terms of the peak value. 256 (2000) = 0db
- band 4 input gain: the input gain of band 4 in terms of the peak value. 256 (2000) = 0db

## group 3: distortion type control
 
- band 1 type: the distortion type of band 1. these are the same as the stock distortion module
- band 2 type: the distortion type of band 2. these are the same as the stock distortion module
- band 3 type: the distortion type of band 3. these are the same as the stock distortion module
- band 4 type: the distortion type of band 4. these are the same as the stock distortion module

## group 4: distortion power control

- band 1 power: the power (gain) of band 1's distortion
- band 2 power: the power (gain) of band 2's distortion
- band 3 power: the power (gain) of band 3's distortion
- band 4 power: the power (gain) of band 4's distortion

## group 5: distortion bit depth control

- band 1 bit depth: the bit depth of band 1. 16 (10) is no change to the bit depth
- band 2 bit depth: the bit depth of band 2. 16 (10) is no change to the bit depth
- band 3 bit depth: the bit depth of band 3. 16 (10) is no change to the bit depth
- band 4 bit depth: the bit depth of band 4. 16 (10) is no change to the bit depth

## group 6: distortion sample rate control

- band 1 freq: the sample rate of band 1 in hertz
- band 2 freq: the sample rate of band 2 in hertz
- band 3 freq: the sample rate of band 3 in hertz
- band 4 freq: the sample rate of band 4 in hertz

## group 7: distortion noise control

- band 1 noise: the noise of band 1. note that this is not the same as adding white noise, this effect adds a random value to each sample
- band 2 noise: the noise of band 2. note that this is not the same as adding white noise, this effect adds a random value to each sample
- band 3 noise: the noise of band 3. note that this is not the same as adding white noise, this effect adds a random value to each sample
- band 4 noise: the noise of band 4. note that this is not the same as adding white noise, this effect adds a random value to each sample