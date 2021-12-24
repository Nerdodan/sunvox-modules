#abstract

this module was inspired by the talkbox guitar effect. here, it is simply a vocal filter modulated by an lfo

#controllers

##group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

##group 2: vocal filter settings

- vowel: the base vowel of the filter
- formant width: the formant width in hertz
- intensity: the gain of the formants
- formants: the number of formants
- voice type: the type of voice

##group 3: lfo settings

- lfo amp: the amplitude of the lfo
- lfo speed: the speed of the lfo in the chosen frequency unit
- lfo waveform: the waveform to use as the lfo
- lfo frequency unit: the frequency unit for the lfo
- lfo duty cycle: the pulsewidth (duty cycle) of the pulse wave lfo

##group 4: additional vocal filter settings

- random frequency: the amount of randomness applied to the formants' frequencies
- random seed: the seed for the formant random frequency
- vowel1, vowel2, etc.: the vowel in the five-vowel sequence
