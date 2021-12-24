# abstract

a simple but versatile phaser effect

the multictl curves were generated using pixilang, i'll see if i can find the original file

# controllers

## group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

## group 2: main settings

- poles: the number of phaser poles. 2048 (800) = one pole
- spread: the resonance of the allpass filters
- feedback: the phaser feedback

## group 3: frequency settings

- min frequency: the minimum possible frequency of the phaser lfo
- max frequency: the maximum possible frequency of the phaser lfo. this controller is what you'll want to adjust if you want to manually automate the phaser frequency

## group 4: lfo settings

- lfo amp: the amplitude of the lfo
- lfo freq: the frequency of the lfo in the frequency unit
- lfo freq unit: the frequency unit of the lfo
- lfo waveform: the waveform of the lfo
- lfo duty cycle: the pulsewidth (duty cycle) of the pulse wave lfo

##group 5: sound2ctl sample rate settings

- lfo sample rate: the sample rate of the sound2ctl module in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot