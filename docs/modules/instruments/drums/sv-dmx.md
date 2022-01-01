# abstract

a "pseudosample-based" drum machine inspired by sample-based drum machines like the oberheim dmx and the roland tr-707. unlike those, all the sounds here are done via synthesis :>

also unlike the original machines, this module comes with a built-in gated reverb unit with prefiltering, for all your 80's drum needs

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

## group 2: dry/wet settings

- gated reverb dry: the gain of the dry signal, 128 (1000) = -6db
- gated reverb wet: the gain of the wet signal, 128 (1000) = -6db

## group 3: hp filter settings

- gated reverb hp freq: the frequency of the highpass filter in hertz
- gated reverb hp q: the resonance of the highpass filter
- gated reverb hp roll-off: the roll-off of the highpass filter in db/oct

## group 4: lp filter settings

- gated reverb lp freq: the frequency of the lowpass filter in hertz
- gated reverb lp q: the resonance of the lowpass filter
- gated reverb lp roll-off: the roll-off of the lowpass filter in db/oct

## group 5: reverb settings

- gated reverb feedback: the feedback of the reverb
- gated reverb damp: the dampening (lowpass filter) of the reverb
- gated reverb width: the width of the reverb. 0 is mono
- gated reverb size: the size of the reverb
- gated reverb seed: the random seed for the reverb

## group 6: gate settings

- gated reverb input gain: the input gain of the signal. 256 (2000) = 0db
- gated reverb threshold: the threshold of the gate in terms of the peak value. 128 (2000) = -6db
- gated reverb slope: the slope (ratio) of the gate curve in percentage. 50 (2000) = 1:2
- gated reverb attack: the attack of the gate in milliseconds
- gated reverb release: the release of the gate in milliseconds
- gated reverb output gain: the output gain of the signal. 256 (2000) = 0db