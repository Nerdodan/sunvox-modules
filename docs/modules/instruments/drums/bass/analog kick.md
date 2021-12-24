# abstract

a module simulating the kick sound produced by many analog drum machines. it works simply by generating a low tone with a pitch and amplitude envelope and some mild saturation

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

# controllers

## group 1: body settings

- body coarse: the coarse pitch of the tone in semitones. 0 (80) = c5
- body fine: the fine pitch of the tone in semitones/256.
- body phase: the starting phase of the tone. 8192 (2000) = pi/2
- body release: the release time of the tone

## group 2: pitch env controls

- pitch env amt: the amount of the pitch envelope. 0 = no pitch envelope
- pitch env release: the release of the pitch envelope

## group 3: saturation controls

- sat input volume: the input gain to the saturator. note that 0 = silence

## group 4: sound2ctl sample rate settings

- envelope sample rate: the sample rate of the sound2ctl module in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot