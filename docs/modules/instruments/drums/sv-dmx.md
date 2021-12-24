# abstract

a "pseudosample-based" drum machine inspired by sample-based drum machines like the oberheim dmx and the roland tr-707. unlike those, all the sounds here are done via synthesis :>

the drum sounds are as follows, starting on note c0:

- c0: kick
- c#0: snare
- d0: sidestick
- d#0: closed hihat
- e0: open hihat
- f0: high tom
- f#0: mid tom
- g0: low tom
- g#0: crash
- a0: ride
- a#0: shaker
- b0: tambourine
- c1: clap

the sounds simply loop around at c#1 and so on

the bit depth of this module is in 12-bit, true to the original machines

if you want to play with the sound generators, all the drum sound modules are available in this repository as well

# controls

## group 1: percussion volume settings

- kick volume: the volume of the kick in terms of the peak level. 16384 (4000) = -6db
- snare volume: the volume of the snare and sidestick in terms of the peak level. 16384 (4000) = -6db
- hihat volume: the volume of the closed and open hihat in terms of the peak level. 16384 (4000) = -6db
- toms volume: the volume of the high, mid, and low toms in terms of the peak level. 16384 (4000) = -6db
- cymbal volume: the volume of the crash and ride in terms of the peak level. 16384 (4000) = -6db
- perc volume: the volume of the shaker, tambourine, and clap in terms of the peak level. 16384 (4000) = -6db