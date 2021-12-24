#abstract

a monophonic phase modulation synthesizer module inspired by native instruments's fm8 plugin

uses true keytracking for the modulation, which means that the waveform will be the same regardless of the pitch. however, as a drawback from this algorithm, bass notes will be distorted if the modulation amount is too high

particularly great for brostep basses, though it can do a wide variety of fm sounds as well

uses a matrix-based routing system, as well as a single controller for the envelopes

the envelope algorithm is as follows, with controller values in decimal and hexadecimal:

- 0 (0): 0 attack, 0 release, sustain on
- 4096 (1000): 0 attack, 256 release, sustain on
- 8192 (2000): 256 attack, 0 release, sustain on
- 12288 (3000): 0 attack, 0 release, sustain on
- 16383 (3fff): 256 attack, 256 release, sustain on
- 16384 (4000): 0 attack, 0 release, sustain off
- 20480 (5000): 0 attack, 256 release, sustain off
- 24576 (6000): 256 attack, 0 release, sustain off
- 28672 (7000): 0 attack, 0 release, sustain off
- 32768 (8000): 256 attack, 256 release, sustain off

#controllers

##group 1: op 1 settings

- op 1 coarse: the coarse detuning from the input pitch for this operator, in semitones
- op 1 fine: the fine detuning from the input pitch for this operator, in semitones/256
- op 1 envelope: the envelope for operator 1
- op 1 waveform: the waveform for operator 1

##group 2: op 2 settings

- op 2 coarse: the coarse detuning from the input pitch for this operator, in semitones
- op 2 fine: the fine detuning from the input pitch for this operator, in semitones/256
- op 2 envelope: the envelope for operator 2
- op 2 waveform: the waveform for operator 2

##group 3: op 3 settings

- op 3 coarse: the coarse detuning from the input pitch for this operator, in semitones
- op 3 fine: the fine detuning from the input pitch for this operator, in semitones/256
- op 3 envelope: the envelope for operator 3
- op 3 waveform: the waveform for operator 3

##group 4: op 4 settings

- op 4 coarse: the coarse detuning from the input pitch for this operator, in semitones
- op 4 fine: the fine detuning from the input pitch for this operator, in semitones/256
- op 4 envelope: the envelope for operator 4
- op 4 waveform: the waveform for operator 4

##group 5: mod matrix

- 4 -> 3 amt: the amount of modulation between operators 4 and 3
- 4 -> 2 amt: the amount of modulation between operators 4 and 2
- 4 -> 1 amt: the amount of modulation between operators 4 and 1
- 3 -> 2 amt: the amount of modulation between operators 3 and 2
- 3 -> 1 amt: the amount of modulation between operators 3 and 1
- 2 -> 1 amt: the amount of modulation between operators 2 and 1

##group 6: operator output

- op 1 out: the output of operator 1 in terms of the peak value. 16384 (4000) = 6db
- op 2 out: the output of operator 2 in terms of the peak value. 16384 (4000) = 6db
- op 3 out: the output of operator 3 in terms of the peak value. 16384 (4000) = 6db
- op 4 out: the output of operator 4 in terms of the peak value. 16384 (4000) = 6db