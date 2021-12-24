# abstract

a module simulating the cymbal sound produced by many analog drum machines. it works by mixing sampled noise and the output of three pairs of pulse waves frequency modulating each other

it can produce analog style crashes, rides, hihats, and more

# controllers

## group 1: overall settings

- noise/metal blend: the blend of the noise and metal components. 16384 (4000) = 50% noise 50% metal

## group 2: envelope settings

- attack: the attack of the amp envelope
- release: the release of the amp envelope
- exponential envelope: enables the exponential mode for the amp envelopes

## group 3: highpass settings

- hp freq: the frequency of the highpass filter in hertz
- hp resonance: the resonance of the highpass filter
- hp roll-off: the roll-off of the highpass filter in db/oct

## group 4: noise settings

- noise phase: the phase (playback position) of the sampled noise

## group 5: pair 1 settings

- car 1 coarse: the coarse pitch of carrier 1 in semitones. 0 (80) = c5
- car 1 fine: the fine pitch of carrier 1 in semitones/256
- mod 1 coarse: the coarse pitch of modulator 1 in semitones. 0 (80) = c5
- mod 1 fine: the fine pitch of modulator 1 in semitones/256
- mod 1 amp: the amplitude of modulator 1 in terms of the peak level. 16384 (4000) = -6db

## group 6: pair 2 settings

- car 2 coarse: the coarse pitch of carrier 2 in semitones. 0 (80) = c5
- car 2 fine: the fine pitch of carrier 2 in semitones/256
- mod 2 coarse: the coarse pitch of modulator 2 in semitones. 0 (80) = c5
- mod 2 fine: the fine pitch of modulator 2 in semitones/256
- mod 2 amp: the amplitude of modulator 2 in terms of the peak level. 16384 (4000) = -6db

## group 7: pair 3 settings

- car 3 coarse: the coarse pitch of carrier 3 in semitones. 0 (80) = c5
- car 3 fine: the fine pitch of carrier 3 in semitones/256
- mod 3 coarse: the coarse pitch of modulator 3 in semitones. 0 (80) = c5
- mod 3 fine: the fine pitch of modulator 3 in semitones/256
- mod 3 amp: the amplitude of modulator 3 in terms of the peak level. 16384 (4000) = -6db

## group 4: sound2ctl sample rate settings

- fm sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot
