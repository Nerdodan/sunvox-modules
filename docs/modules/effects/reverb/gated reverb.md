# abstract

a variant of the reverb module with a built-in gate, also features prefiltering

# controllers

## group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

## group 2: hp filter settings

- hp freq: the frequency of the highpass filter in hertz
- hp q: the resonance of the highpass filter
- hp roll-off: the roll-off of the highpass filter in db/oct

## group 3: lp filter settings

- lp freq: the frequency of the lowpass filter in hertz
- lp q: the resonance of the lowpass filter
- lp roll-off: the roll-off of the lowpass filter in db/oct

## group 4: reverb settings

- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb width: the width of the reverb. 0 is mono
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb

## group 5: gate settings

- gate input gain: the input gain of the signal. 256 (2000) = 0db
- gate threshold: the threshold of the gate in terms of the peak value. 128 (2000) = -6db
- gate slope: the slope (ratio) of the gate curve in percentage. 50 (2000) = 1:2
- gate attack: the attack of the gate in milliseconds
- gate release: the release of the gate in milliseconds
- gate output gain: the output gain of the signal. 256 (2000) = 0db