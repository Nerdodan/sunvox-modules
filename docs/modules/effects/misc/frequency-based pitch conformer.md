# abstract

this module takes two inputs: the audio and the note to conform to. the module detects the pitch of the audio, calculates the difference between that and the input note pitch, and pitch shifts the audio down to the desired pitch

use it for vocal pitch correction (where the notes of the melody are the note input alongside the audio), or for wild detuning/autotune effects

# controllers

## group 1: pitch detector settings

- detector algorithm: the algorithm to use for pitch detection. cepstrum works better on high notes and vice versa
- detector threshold: the threshold for the pitch detection. anything below it is ignored
- detector alg1-2 sample rate: the sample rate for the autocorrelation and cepstrum algorithms
- detector alg1-2 buffer: the buffer for the autocorrelation and cepstrum algorithms in milliseconds
- detector alg1-2 overlap: the overlap for the autocorrelation and cepstrum algorithms in percentage
- detector alg1 absolute threshold: the absolute threshold for the autocorrelation algorithm

## group 2: pitch shifter settings

- pitch shifter grain size: the grain size of the pitch shifter

## group 3: additional settings

- gate mode: whether to gate the audio output based on note input