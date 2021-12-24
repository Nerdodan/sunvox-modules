# abstract

a percussion module designed to generate drum sounds reminiscent of old computer chips via amplitude and frequency modulation. it works by generating three waveforms with an asr envelope and frequency modulating the first by the second and amplitude modulating the first by the third

for a kit-based variant of this module, please see my chip perc kit module

great as percussion for music genres like idm and glitch

# controls

## group 1: pitch control

- input pitch: the overall pitch of the sound in semitones/10. 0 = C5
- main pitch: the pitch of the main waveform in semitones/10. 0 = C5
- amp pitch: the pitch of the amplitude modulating waveform in semitones/10. 0 = C5
- freq pitch: the pitch of the frequency modulating waveform in semitones/10. 0 = C5

## group 2: waveform control

- main osc: the main oscillator, based on the generator module's waveforms. note that the "drawn" waveform is simply a dc signal, for creating envelopes.
- amp osc: the amplitude modulating oscillator, based on the generator module's waveforms. note that the "drawn" waveform is simply a dc signal, for creating envelopes.
- freq osc: the frequency modulating oscillator, based on the generator module's waveforms. note that the "drawn" waveform is simply a dc signal, for creating envelopes.

## group 3: attack control

- main attack: the attack of the main oscillator in seconds/256. maximum is two seconds
- amp attack: the attack of the amplitude modulating oscillator in seconds/256. maximum is two seconds
- freq attack: the attack of the frequency modulating oscillator in seconds/256. maximum is two seconds

## group 3: release control

- main release: the release of the main oscillator in seconds/256. maximum is two seconds
- amp release: the release of the amplitude modulating oscillator in seconds/256. maximum is two seconds
- freq release: the release of the frequency modulating oscillator in seconds/256. maximum is two seconds

## group 4: sustain control

- main sustain: whether to enable sustain on the main oscillator
- amp sustain: whether to enable sustain on the amplitude modulating oscillator
- freq sustain: whether to enable sustain on the frequency modulating oscillator

## group 5: amplitude modulation settings

- min amp: the minimum amplitude for the amplitude modulation in terms of the peak level. 16384 (4000) = -6db
- max amp: the maximum amplitude for the amplitude modulation in terms of the peak level. 16384 (4000) = -6db

## group 6: frequency modulation settings

- min freq: the minimum pitch for the frequency modulation relative to the main oscillator's pitch. 16384 (4000) = the base pitch
- max freq: the maximum pitch for the frequency modulation relative to the main oscillator's pitch. 16384 (4000) = the base pitch

## group 7: absoulte value settings

- amp absolute: whether to take the absolute value of the amplitude modulation oscillator
- freq absolute: whether to take the absolute value of the frequency modulation oscillator

## group 8: sound2ctl sample rate settings

- envelope sample rate: the sample rate of the sound2ctl module in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot