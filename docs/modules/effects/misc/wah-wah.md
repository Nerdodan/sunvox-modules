# abstract

a wah-wah effect. the effect can be controlled in three ways: auto (following the signal amplitude), manually (adjusting the manual frequency), or by lfo

# controllers

## group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

## group 2: auto settings

- auto: enables auto mode
- auto min: the minimum frequency of the envelope follower
- auto max: the maximum frequency of the envelope follower

## group 3: manual settings

- manual freq: the manual frequency of the effect. if you have a midi pedal on hand, you could map the output cc to this controller and replicate a real wah pedal
- manual response: the response of the effect. 1000 (8000) is instantaneous response

## group 4: lfo settings

- lfo amp: the amplitude of the lfo
- lfo speed: the speed of the lfo in the chosen frequency unit
- lfo waveform: the waveform to use as the lfo
- lfo frequency unit: the frequency unit for the lfo
- lfo duty cycle: the pulsewidth (duty cycle) of the pulse wave lfo

## group 5: filter settings

- filter type: the type of filter to use
- filter bandwidth: the resonance (bandwidth) of the filter
- filter roll-off: the roll-off of the filter in db/oct
- filter gain: the gain of the filter from -24db to +24db

## group 6: sound2ctl sample rate settings

- auto/lfo sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot
