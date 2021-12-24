# abstract

an 8-voice polyphonic analog-style synthesizer module inspired by the roland juno 6, oberheim ob-x, and others

for each voice, two oscillators are detuned, mixed, and sent to a highpass and lowpass filter. the lowpass filter can be modulated by the envelope or lfo or both. the amplitude is then modulated by either the main adsr envelope or a gate envelope. the pitch and pulsewidth can also be modulated by the lfo and the envelope in the case of the pulsewidth. the voices are sent to two parallel chorus units, which cam be crossfaded

as of 2.0, this module uses cyclic round-robin-based voice allocation

though this succeeds my analog synth module, it does not replace it; they coexist

great for all your retro analog polysynth sound needs

note that the waveforms are controlled by a multictl, so the individual waveform names are not available. they are the same as the analog generator, minus the harmonics waveform, and are as follows, with decimal and hexadecimal values:

- 0 (0): triangle
- 2048 (800): saw
- 4096 (1000): pulse
- 6144 (1800): noise (sampler)
- 8192 (2000): drawn
- 10240 (2800): sin
- 12288 (3000): hsin
- 14336 (3800): asin
- 16384 (4000): drawn spline
- 18432 (4800): noise spline (sampler)
- 20480 (5000): white noise
- 22528 (5800): pink noise
- 24768 (6000): red noise
- 26624 (6800): blue noise
- 28672 (7000): violet noise
- 30720 (7800): grey noise

# controllers

## group 1: lfo + pwm settings

- lfo speed: the speed of the voice lfos
- lfo attack: the attack time of the voice lfos
- vibrato: the amount of pitch modulation by the lfo
- portamento: the amount of portamento between notes
- pulse width: the base pulsewidth (duty cycle) of the pulse waveform
- pwm amount: the amount of pulsewidth modulation of the pulse waveform
- pwm lfo/env mix: the mixture between the lfo and envelope for the pwm

## group 2: oscillator settings

- osc 1 range: the octave offset of oscillator 1. 8192 (2000) = +0 octaves
- osc 1 waveform: the waveform for oscillator 1
- osc 2 range: the octave offset of oscillator 2. 8192 (2000) = +0 octaves
- osc 2 finetune: the finetune of oscillator 2 in semitones/16384
- osc 2 waveform: the waveform for oscillator 2
- osc mix: the mixture of oscillators 1 and 2. 16384 (4000) = 50% osc 1 50% osc 2

## group 3: filter settings

- hp cutoff: the exponential frequency of the 12db highpass filter
- lp cutoff: the exponential frequency of the lowpass filter at the maximum velocity
- lp resonance: the resonance of the lowpass filter
- lp 24db: enables 24db mode for the lowpass filter. 12db when it is off
- lp env amount: the amount of the envelope on the filter frequency
- lp lfo amount: the amount of the lfo on the filter frequency

## group 4: envelope settings

- amp gate mode: enables gate mode for the envelope. this enables sustain on note on and off on note off, with no attack or release
- attack: the attack of the envelope
- decay: the decay of the envelope
- sustain level: the sustain level of the main envelope
- release: the release of the envelope

## group 5: effect settings

- chorus wet: the amount (wet) of the chorus effect. 16384 (4000) = -6db
- chorus mix: the mixture between choruses 1 and 2
- stereo width: the width of the chorus output