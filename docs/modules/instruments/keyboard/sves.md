# abstract

a clone of the programmable sound generators in the famicom/nintendo entertainment system. "sves" stands for "sunvox entertainment system" :>

it uses two pulse waves with quantized but variable pulse width, a 4-bit triangle wave, 1-bit noise, and a 7-bit/15khz pcm (sample) player

every generator has four global modulators: a coarse (+/- 12 semtiones) and fine (+/- 1 semitone) pitch envelope/lfo, an amplitude envelope/lfo, and in the case of the pulse waves, a pwm envelope/lfo. the envelopes/lfo can be mixed together

each generator can be enabled by setting the input module controller to 2-6, or they can all be used at once via channel division by setting the input module controller to 1

note that you will need to go inside the module to set the pcm waveform, though there is no need to crush it to 7-bit/15khz yourself. by default it is the observer.xi waveform from sunvox's included instruments

be sure to adjust the module bpm to your taste if the lfo frequency units are set to a musical value!

# controllers

## group 1: response controls

- velocity sensing: enables velocity sensing
- portamento: enables portamento. 0 is no portamento (instantaneous response)

## group 2: generator mix

- pulse 1 mix: the volume of pulse 1 in terms of the peak value. 16384 (4000) = -12db
- pulse 1 balance: the panning of pulse 1. 0 = center (mono)
- pulse 2 mix: the volume of pulse 2 in terms of the peak value. 16384 (4000) = -12db
- pulse 2 balance: the panning of pulse 2. 0 = center (mono)
- triangle mix: the volume of the triangle in terms of the peak value. 16384 (4000) = -12db
- triangle balance: the panning of the triangle. 0 = center (mono)
- noise mix: the volume of the noise in terms of the peak value. 16384 (4000) = -12db
- noise balance: the panning of the noise. 0 = center (mono)
- pcm mix: the volume of the pcm waveform in terms of the peak value. 16384 (4000) = -12db
- pcm balance: the panning of the pcm waveform. 0 = center (mono)

## group 3: coarse pitch modulation controls

- pitch env/lfo mix: the mixture between the envelope and the lfo
- pitch send vol: the amount of modulation to apply
- pitch send offset: the offset of the modulator
- pitch send quantization: the quantization of the modulator in bits
- pitch env attack: the attack of the envelope in milliseconds
- pitch env decay: the decay of the envelope in milliseconds
- pitch env sustain: the sustain mode of the envelope
- pitch env sustain level: the sustain level of the envelope
- pitch env release: the release of the envelope in milliseconds
- pitch lfo freq: the frequency of the lfo in terms of the chosen frequency unit
- pitch lfo waveform: the waveform of the lfo
- pitch lfo duty cycle: the pulsewidth (duty cycle) of the lfo in the case of the pulse wave
- pitch lfo frequency unit: the frequency unit of the lfo

## group 4: fine pitch modulation controls

- fine pitch env/lfo mix: the mixture between the envelope and the lfo
- fine pitch send vol: the amount of modulation to apply
- fine pitch send offset: the offset of the modulator
- fine pitch send quantization: the quantization of the modulator in bits
- fine pitch env attack: the attack of the envelope in milliseconds
- fine pitch env decay: the decay of the envelope in milliseconds
- fine pitch env sustain: the sustain mode of the envelope
- fine pitch env sustain level: the sustain level of the envelope
- fine pitch env release: the release of the envelope in milliseconds
- fine pitch lfo freq: the frequency of the lfo in terms of the chosen frequency unit
- fine pitch lfo waveform: the waveform of the lfo
- fine pitch lfo duty cycle: the pulsewidth (duty cycle) of the lfo in the case of the pulse wave
- fine pitch lfo frequency unit: the frequency unit of the lfo

## group 5: pwm modulation controls

- pwm env/lfo mix: the mixture between the envelope and the lfo
- pwm send vol: the amount of modulation to apply
- pwm send offset: the offset of the modulator
- pwm send quantization: the quantization of the modulator in bits. note that the original console had 4 levels of pwm, so set this to 2 bits for more realism
- pwm env attack: the attack of the envelope in milliseconds
- pwm env decay: the decay of the envelope in milliseconds
- pwm env sustain: the sustain mode of the envelope
- pwm env sustain level: the sustain level of the envelope
- pwm env release: the release of the envelope in milliseconds
- pwm lfo freq: the frequency of the lfo in terms of the chosen frequency unit
- pwm lfo waveform: the waveform of the lfo
- pwm lfo duty cycle: the pulsewidth (duty cycle) of the lfo in the case of the pulse wave
- pwm lfo frequency unit: the frequency unit of the lfo

## group 6: amplitude modulation controls

- amp env/lfo mix: the mixture between the envelope and the lfo
- amp send vol: the amount of modulation to apply
- amp send offset: the offset of the modulator
- amp send quantization: the quantization of the modulator in bits. note that the original console had 15 levels of amplitude, so set this to 4 bits for more realism
- amp env attack: the attack of the envelope in milliseconds
- amp env decay: the decay of the envelope in milliseconds
- amp env sustain: the sustain mode of the envelope
- amp env sustain level: the sustain level of the envelope
- amp env release: the release of the envelope in milliseconds
- amp lfo freq: the frequency of the lfo in terms of the chosen frequency unit
- amp lfo waveform: the waveform of the lfo
- amp lfo duty cycle: the pulsewidth (duty cycle) of the lfo in the case of the pulse wave
- amp lfo frequency unit: the frequency unit of the lfo

## group 7: sound2ctl sample rate settings

- sound2ctl sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot