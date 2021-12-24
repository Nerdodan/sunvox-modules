# abstract

an attempt to simulate the sound of chanting choirs, with a synthetic twist

uses a random envelope on the vocal filter vowel, as well as random consonants (noise) at the beginning and end of each note

also comes with a built-in hall reverb unit

# controllers

## group 1: vocal filter settings

- voice type: the type of voice for the vocal filter
- formants: the number of formants in the vocal filter

## group 2: additional vocal settings

- consonant volume: the maximum volume of the consonants in terms of the peak level. 16384 (4000) = -6db
- vowel shift speed: the speed of the random vowel shift in milliseconds

## group 3: envelope settings

- attack: the attack of the amplitude envelope
- release: the release of the amplitude envelope
- sustain: enables the sustain of the amplitude envelope

## group 4: physical settings

- voice seed: sets the random seed for the voice resonator

## group 5: hall reverb settings

- hall reverb wet: the volume of the reverb (wet) signal. 128 (4000) = -6db
- hall reverb feedback: the feedback of the reverb
- hall reverb damp: the dampening (lowpass filter) of the reverb
- hall reverb width: the width of the reverb. 0 is mono
- hall reverb mode: the mode of the reverb
- hall reverb size: the size of the reverb
- hall reverb seed: the random seed for the reverb

## group 4: sound2ctl sample rate settings

- sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot