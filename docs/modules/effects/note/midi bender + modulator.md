# abstract

this module allows you to perform pitch bend and pitch modulation effects on notes. not only that, but the two controllers are by default mapped to the midi pitch bend and modulation ccs, so they should work with any midi keyboard

# controllers

## group 1: core effects

- pitch bend: bends the pitch of the note up or down by the specified scale
- pitch mod: modulates the pitch of the note up and down by the specified scale

## group 2: pitch bend settings

- pitch bend response: the response of the pitch bending. 1000 (8000) is instantaneous response
- pitch bend scale: the scaling of the pitch bend in percentage. 4% = +-2 semitones

## group 3: pitch mod settings

- pitch mod response: the response of the pitch modulation. 1000 (8000) is instantaneous response
- pitch mod scale: the scaling of the pitch modulation in percentage. 4% = +-2 semitones
- pitch mod lfo speed: the speed of the modulation lfo by the frequency unit
- pitch mod lfo wave: the waveform of the modulation lfo
- pitch mod lfo unit: the frequency unit for the lfo
- pitch mod lfo duty cycle: the pulsewidth (duty cycle) of the pulse wave lfo

## group 4: sound2ctl sample rate settings

- lfo sample rate: the sample rate of the sound2ctl module in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot
