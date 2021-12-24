# abstract

a four-band variant of my saturator module

saturates each band separately and sums the bands

uses inversion-based band splits to negate phase coloration

the waveshaper curves were generated using pixilang, i'll see if i can find the original file

# controllers

## group 1: band split controls

- band 1/2 split: the split frequency of bands 1 and 2 in hertz
- band 2/3 split: the split frequency of bands 2 and 3 in hertz
- band 3/4 split: the split frequency of bands 3 and 4 in hertz

## group 2: input gain controls

- band 1 input gain: the input gain of band 1 in terms of the peak value. 256 (2000) = 0db
- band 2 input gain: the input gain of band 2 in terms of the peak value. 256 (2000) = 0db
- band 3 input gain: the input gain of band 3 in terms of the peak value. 256 (2000) = 0db
- band 4 input gain: the input gain of band 4 in terms of the peak value. 256 (2000) = 0db

## group 3: odd/even harmonics controls

- band 1 odd/even harmonics: the mix of the symmetrical/asymmetrical saturators on band 1
- band 2 odd/even harmonics: the mix of the symmetrical/asymmetrical saturators on band 2
- band 3 odd/even harmonics: the mix of the symmetrical/asymmetrical saturators on band 3
- band 4 odd/even harmonics: the mix of the symmetrical/asymmetrical saturators on band 4

## group 4: character controls

- band 1 character: the curve shape of the saturator on band 1
- band 2 character: the curve shape of the saturator on band 2
- band 3 character: the curve shape of the saturator on band 3
- band 4 character: the curve shape of the saturator on band 4

## group 5: mix controls

- band 1 mix: the dry/wet mix of the saturation on band 1. 16384 (4000) = 50% dry 50% wet
- band 2 mix: the dry/wet mix of the saturation on band 2. 16384 (4000) = 50% dry 50% wet
- band 3 mix: the dry/wet mix of the saturation on band 3. 16384 (4000) = 50% dry 50% wet
- band 4 mix: the dry/wet mix of the saturation on band 4. 16384 (4000) = 50% dry 50% wet
