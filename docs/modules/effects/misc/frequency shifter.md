# abstract

a simple bode frequency shifter using donald k. weaver's single sideband modulation method. the new fft module is used as the lowpass filter here

this is different from pitch shifting in that the frequencies are shifted linearly (in hertz) rather than exponentially (in semitones or another pitch unit). the effect is quite similar to ring modulation in terms of the sound

this affects both stereo channels the same way. use two in parallel with different settings for each channel for interesting stereo effects

this does do some weird phase smearing for some reason, but i suppose that isn't an issue if you just want cool frequency effects

# controllers

## group 1: main settings

- shift: the shift in hertz/2