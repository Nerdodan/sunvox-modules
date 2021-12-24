#abstract

a four-band variant of my limiter module

limits each band separately and sends the bands to a brickwall limiter

uses inversion-based band splits to negate phase coloration

to get that sweet "fuck dynamic range" effect, just crank up all the input gain controllers to your liking. not recommended if you want to treat your listeners like human beings

#controllers

##group 1: band split

- band 1/2 split: the split frequency of bands 1 and 2 in hertz
- band 2/3 split: the split frequency of bands 2 and 3 in hertz
- band 3/4 split: the split frequency of bands 3 and 4 in hertz

##group 2: input volume control

- band 1 input volume: the input gain of band 1 in terms of the peak value. 256 (2000) = 0db
- band 2 input volume: the input gain of band 2 in terms of the peak value. 256 (2000) = 0db
- band 3 input volume: the input gain of band 3 in terms of the peak value. 256 (2000) = 0db
- band 4 input volume: the input gain of band 4 in terms of the peak value. 256 (2000) = 0db

##group 3: threshold control

- band 1 threshold: the threshold of band 1's limiter in terms of the peak value. 128 (2000) = -6db
- band 2 threshold: the threshold of band 2's limiter in terms of the peak value. 128 (2000) = -6db
- band 3 threshold: the threshold of band 3's limiter in terms of the peak value. 128 (2000) = -6db
- band 4 threshold: the threshold of band 4's limiter in terms of the peak value. 128 (2000) = -6db

##group 4: attack control

- band 1 attack: the attack of band 1's limiter in milliseconds
- band 2 attack: the attack of band 2's limiter in milliseconds
- band 3 attack: the attack of band 3's limiter in milliseconds
- band 4 attack: the attack of band 4's limiter in milliseconds

##group 5: release control

- band 1 release: the release of band 1's limiter in milliseconds
- band 2 release: the release of band 2's limiter in milliseconds
- band 3 release: the release of band 3's limiter in milliseconds
- band 4 release: the release of band 4's limiter in milliseconds

##group 6: brickwall control

- threshold: the threshold of the brickwall limiter in terms of the peak value. 128 (2000) = -6db
- release: the release of the brickwall limiter in milliseconds

##group 7: overall settings

- lookahead time: the lookahead time of the lookahead limiters in milliseconds
