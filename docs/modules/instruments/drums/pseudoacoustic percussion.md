# abstract

this module allows you to synthesize the sound of a plastic bin being used as a percussion instrument, as well as bins of other materials like wood or metal

it uses a sine wave generator and a sampled noise generator with a comb filter and a highpass/lowpass combo, both sent into two resonators

use it to make interesting percussions for your music, or just to synthesize a mayonnaise jar because why not

# controllers

## group 1: overall settings

- all transpose: the base pitch of both the sine wave and sampled noise in semitones. 0 (80) = c5

## group 2: tone settings

- tone transpose: the pitch of the sine wave relative to the overall pitch in semitones. 0 (80) = the base pitch
- tone release: the release of the sine wave
- tone amp: the amplitude of the sine wave in terms of the peak level. 16384 (4000) = -6db

## group 3: noise settings

- noise transpose: the pitch of the sampled noise relative to the overall pitch in semitones. 0 (80) = the base pitch. lower values give a sample rate reduction effect
- noise phase: the phase (playback position) of the sampled noise
- noise release: the release of the sampled noise
- noise comb wet: the amount of comb filtered (wet) signal. 128 (4000) = -6db
- noise comb delay: the delay of the comb filter in milliseconds. maximum delay is one second
- noise comb feedback: the feedback of the comb filter
- noise lp freq: the frequency of the lowpass filter in hertz
- noise hp freq: the frequency of the highpass filter in hertz
- noise amp: the amplitude of the sampled noise in terms of the peak level. 16384 (4000) = -6db

## group 4: resonator 1 settings

- resonator 1 wet: the amount of the resonated (wet) signal. 128 (4000) = -6db
- resonator 1 feedback: the feedback of the resonator
- resonator 1 damp: the dampening (lowpass filter) of the resonator.
- resonator 1 mode: the mode of the resonator
- resonator 1 allpass: enables the allpass filter in the resonator. makes the sound smoother and more smeared
- resonator 1 size: the size of the resonator
- resonator 1 seed: the random seed for the resonator

## group 5: resonator 2 settings

- resonator 2 wet: the amount of the resonated (wet) signal. 128 (4000) = -6db
- resonator 2 feedback: the feedback of the resonator
- resonator 2 damp: the dampening (lowpass filter) of the resonator.
- resonator 2 mode: the mode of the resonator
- resonator 2 allpass: enables the allpass filter in the resonator. makes the sound smoother and more smeared
- resonator 2 size: the size of the resonator
- resonator 2 seed: the random seed for the resonator