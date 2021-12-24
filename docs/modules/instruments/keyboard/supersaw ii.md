# abstract

a version of the analog generator with up to eight voices of unison with detune, blend, random phase, and stereo spread, as well as sixteen voices of polyphony

along with the classic supersaw sound, you can also use this to create many more types of ~~beehives~~ unison sounds and almost anything that the analog generator is capable of doing

while this supercedes my original supersaw modules, they are still maintained because the cpu usage of this module may be too much for some users

the multictl curves in this module were generated using pixilang. i'll see if i can find the original file somewhere

note that the waveforms are controlled by a multictl, so the individual waveform names are not available. they are the same as the analog generator and are as follows, with decimal and hexadecimal values:

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
- 32768 (8000): harmonics

# controllers

## group 1: unison settings

- voices: the number of unison voices. ranges from one to eight
- detune: the detune of the voices. maximum detune means the outermost voices are detuned by one semitone
- random phase: the amount of phase randomness for each voice
- blend: the volume of the non-center voices
- stereo spread: the stereo spread of the voices. minimum spread means the voices are all mono, and maximum spread means the outermost voices are hard panned left and right

## group 2: waveform settings

- waveform: the waveform oscillator

## group 3: amp envelope settings

- attack: the attack of the amp envelope
- release: the release of the amp envelope
- sustain: enables the amp envelope sustain

## group 4: oscillator settings

- duty cycle: the pulsewidth (duty cycle) of the pulse waveform
- osc2 freq: the pitch of the second oscillator relative to the input pitch in semitones/1048.576. 0 means the second oscillator is disabled

## group 5: filter settings

- lp: enables the lowpass filter
- lp cutoff: the exponential cutoff of the lowpass filter
- lp resonance: the resonance of the lowpass filter
- lp 24db: enables 24db roll-off for the lowpass filter. disabled is 12db
- lp attack: the attack of the lowpass filter envelope
- lp release: the release of the lowpass filter envelope
- lp sustain: enables the lowpass filter envelope sustain
- lp envelope: enables the lowpass filter envelope
- hp cutoff: the cutoff of the 12db highpass filter in hertz

## group 6: additional settings

- noise: the volume of the voice white noise in terms of the peak level. 16384 (4000) = -6db
- stereo width: the stereo width of the output

## group 7: osc2 settings

- osc2 volume: the volume of the voice second oscillator in terms of the peak level. 16384 (4000) = -6db
- osc2 mode: the mix mode of the voice second oscillator. these are the same as the analog generator, and are as follows, in decimal and hexadecimal:

- - 0 (0): add
- - 5461 (1555): sub
- - 10923 (2aaa): mul
- - 16384 (4000): min
- - 21845 (5555): max
- - 27307 (6aaa): bitwise and
- - 32768 (8000): bitwise xor