#abstract

an extended version of the reverb module

great for making wide, morphing soundscapes or just regular reverb with some added adjustments

#controllers

##group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

##group 2: predelay settings

- predelay l: the delay on the left channel in milliseconds
- predelay r: the delay on the righ channel in milliseconds
- volume l: the volume of the left channel. 128 (4000) = -6db
- volume r: the volume of the right channel. 128 (4000) = -6db

##group 3: filter settings

- hp freq: the frequency of the highpass filter in hertz
- hp q: the resonance of the highpass filter
- hp roll-off: the roll-off of the highpass filter in db/oct
- lp freq: the frequency of the lowpass filter in hertz
- lp q: the resonance of the lowpass filter
- lp roll-off: the roll-off of the lowpass filter in db/oct

##group 4: reverb settings

- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb width: the width of the reverb. 0 is mono
- reverb mode: the mode of the reverb
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb

##group 5: pitch shifter settings

- shifter volume: the volume of the parallel pitch shifter. 128 (4000) = 0db
- shifter pitch: the pitch shift in semitones/10
- shifter feedback: the feedback of the pitch shifter
- shifter size: the grain size of the pitch shifter

##group 6: lfo settings

- lfo type: the type of modulation to apply
- lfo amp: the amplitude of the lfo
- lfo freq: the frequency of the lfo in the chosen frequency unit
- lfo waveform: the waveform of the lfo
- lfo frequency unit: the frequency unit of the lfo
- lfo duty cycle: the pulsewidth (duty cycle) of the pulse wave lfo