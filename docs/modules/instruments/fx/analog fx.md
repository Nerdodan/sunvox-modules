#abstract

a module for generating modular-synth-esque effects, inspired by the ems synthi aks. it implements two static oscillators, which can be ring and frequency modulated, which are sent to an lfo filter and reverb

great for making anything from retro sound effects to otherworldly soundscapes

note than when the input module is set to 1, the module will generate its sound only when a note on message is sent. when the input module is set to 2, the first oscillator is replaced with an audio input, allowing you to layer your audio and the second oscillator's output, and send it through the ring modulator, filter, and reverb

#controllers

##group 1: main osc 1 settings

- osc 1 pitch: the pitch of main oscillator 1 in semitones/256. 16384 (4000) = c5
- osc 1 volume: the amplitude of main oscillator 1 in terms of the peak level. 16384 (4000) = -6db
- osc 1 waveform: the waveform for main oscillator 1

##group 2: main osc 2 settings

- osc 2 pitch: the pitch of main oscillator 2 in semitones/256. 16384 (4000) = c5
- osc 2 volume: the amplitude of main oscillator 2 in terms of the peak level. 16384 (4000) = -6db
- osc 2 waveform: the waveform for main oscillator 2

##group 3: fm osc 1 settings

- fm osc 1 pitch: the pitch of fm oscillator 1 in semitones/256. 16384 (4000) = c5
- fm osc 1 volume: the amplitude of fm oscillator 1 in terms of the peak level. 16384 (4000) = -6db
- fm osc 1 waveform: the waveform for fm oscillator 1

##group 4: fm osc 2 settings

- fm osc 2 pitch: the pitch of fm oscillator 2 in semitones/256. 16384 (4000) = c5
- fm osc 2 volume: the amplitude of fm oscillator 2 in terms of the peak level. 16384 (4000) = -6db
- fm osc 2 waveform: the waveform for fm oscillator 2

##group 5: ring osc 1 settings

- ring osc 1 pitch: the pitch of ring oscillator 1 in semitones/256. 16384 (4000) = c5
- ring osc 1 volume: the amplitude of ring oscillator 1 in terms of the peak level. 16384 (4000) = -6db
- ring osc 1 waveform: the waveform for ring oscillator 1

##group 6: ring osc 2 settings

- ring osc 2 pitch: the pitch of ring oscillator 2 in semitones/256. 16384 (4000) = c5
- ring osc 2 volume: the amplitude of ring oscillator 2 in terms of the peak level. 16384 (4000) = -6db
- ring osc 2 waveform: the waveform for ring oscillator 2

##group 7: filter main settings

- filter freq: the exponential frequency of the filter
- filter q: the resonance of the filter
- filter type: the type of filter to use
- filter roll-off: the roll-off of the filter in db/oct

##group 8: filter osc settings

- filter osc pitch: the pitch of the filter oscillator in semitones/256. 16384 (4000) = c5
- filter osc volume: the amplitude of the filter oscillator in terms of the peak level. 16384 (4000) = -6db
- filter osc waveform: the waveform for the filter oscillator

##group 9: reverb settings

- reverb wet: the volume of the reverb (wet) signal. 128 (4000) = -6db
- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb size: the width of the reverb. 0 is mono
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb