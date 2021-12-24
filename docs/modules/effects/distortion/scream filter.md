# abstract

a clone of the scream filter from native instruments's massive, widely used in electronic dance music to make screeching basses

it applies a lowpass filter and a heavily distorted narrow bandpass filter in parallel, whose peak can be keytracked

this comes with three additional controls for the filter roll-off and response, which could be useful for automation

this module accepts note and audio input

# controllers

## group 1: main controls

- freq: the exponential cutoff of the lowpass filter
- resonance: the peak boost of the bandpass filter
- scream: the pitch of the bandpass filter. this adjusts both the static pitch and the offset of the keytracked pitch

## group 2: additional controls

- filter roll-off: the roll-off of the lowpass filter in db/oct
- freq response: the response of the lowpass filter. 1000 (8000) is instantaneous response
- scream response: the response of the bandpass filter. 1000 (8000) is instantaneous response

