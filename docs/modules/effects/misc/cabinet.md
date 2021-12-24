# abstract

this is a guitar cabinet effect

it uses a set of peak filters for the overall shape and the reverb module set to a very low room size for fine details, as well as a room reverb

note that the room reverb is not meant to simulate an amplifier's reverb knob, but rather to simulate the room the amplifier is in

this module uses two mono reverb modules on each channel to negate weird stereo effects

# controllers

## group 1: dry/wet controls

- dry: the dry amount of fine details (low size reverb) in the signal. 32768 (8000) = 0db
- wet: the wet amount of fine details (low size reverb) in the signal. 32768 (8000) = 0db

## group 2: cabinet controls

- cabinet seed: the random seed for the fine details (low size reverb)

## group 3: shape controls

- bass: the gain of the bass peak. has a range of -24 <-> +24 db. this is set to 80 hertz
- mid: the gain of the mid peak. has a range of -24 <-> +24 db. this is set to 814 hertz. note that by default the gain is all the way down because i think it sounds better
- treble: the gain of the treble peak. has a range of -24 <-> +24 db. this is set to 2589 hertz
- presence: the gain of the presence peak. has a range of -24 <-> +24 db. this is set to 13700 hertz

## group 4: room reverb controls

- room wet: the amount of wet signal. 256 (8000) = 0db
- room feedback: the feedback of the room reverb
- room damp: the dampening (lowpass filter) of the room reverb
- room width: the stereo width of the room reverb. 0 is mono
- room size: the size of the room reverb
- room seed: the random seed of the room reverb
