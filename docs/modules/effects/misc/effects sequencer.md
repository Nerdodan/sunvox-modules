#abstract

this module allows you to enable various effects using the keyboard keys. the module does nothing until you input a note

the effects are as follows, starting on note c0:

c0: modulator
c#0: tape stop
d0: retrigger (loop)
d#0: reverse
e0: stretch
f0: distortion
f#0: reverb
g0: compressor

the effects loop around on note g#0 and so on

use this for sequencing glitch effects for your audio. make sure to set the bpm and/or tpl the same as your main project

the modulator uses an lfo connected to an amplitude and phase modulator

the tape stop simply reduces the pitch and gain of the signal until the signal is 0

the reverse and stretch use a delay modulated by a sawtooth wave. the stretch's lfo speed is much slower than the reverse's lfo speed. if you set the correct values, you can do either effect on either of these

the reverb effect actually gates the input to a reverb module, so that the reverb tail will continue even after the note is off

this module's inner workings are laid out so you can exchange effect orders or add your own effects! just be sure to connect the note input to your effect

note that the modulator, tape stop, retrigger, reverse, and stretch reset when consecutive notes are received

#controllers

##group 1: modulator settings

- modulator freq: the frequency of the modulator lfo
- modulator volume: the volume of the modulator lfo. 256 (8000) is maximum lfo effect
- modulator waveform: the waveform of the modulator lfo
- modulator frequency unit: the frequency unit of the modulator lfo
- modulation type: the type of modulation to apply to the signal

##group 2: tape stop settings

- tape stop speed: the speed of the tape stop in milliseconds

##group 3: retrigger settings

- retrigger delay: the delay length of the retrigger in tracker lines
- retrigger repeats: the number of repeats of the retrigger
- retrigger mode: the mode for the retrigger

##group 4: reverse

- reverse unit: the unit for the reverse lfo. a musical value is probably what you want
- reverse speed: the speed of the reverse lfo in percentage

##group 5: stretch

- stretch unit: the unit for the stretch lfo. a musical value is probably what you want
- stretch speed: the speed of the stretch lfo in percentage

##group 6: distortion

- distortion type: the type of distortion
- distortion power: the power (gain) of the distortion
- distortion bits: the bit depth of the distorted signal
- distortion freq: the sample rate of the distorted signal in hertz
- distortion noise: the noise of the distorted signal. note that this is not the same as adding white noise, this effect adds a random value to each sample

##group 7: reverb

- reverb wet: the gain of the wet reverb signal. 32768 (8000) = 0db
- reverb dry: the gain of the dry reverb signal. 32768 (8000) = 0db
- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb size: the size of the reverb

##group 8: compressor

- compressor threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- compressor slope: the slope (ratio) of the compressor curve in percentage. 50 (2000) = 1:2
- compressor attack: the attack of the compressor in milliseconds
- compressor release: the release of the compressor in milliseconds
- compressor makeup gain: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db

