# abstract

a module that allows you to synthesize those huge synthetic kick drums heard in modern electronic music and electronic dance music

based on au5's great tutorial on synthesizing snares and kicks, available [here](https://www.youtube.com/watch?v=ra-mZivYchk)

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

the equalization is based on the default eq module

the compression is based on my compressor pro module. note that the slope is fixed to 100 (1:infinity)

# controllers

## group 1: body settings

- body base freq: the base frequency of the body in semitones. 0 (80) = c5
- body attack: the attack of the body. you'll want to have this at around 50-70 to make room for the transient
- body release: the release of the body
- body exponential envelope: enables the exponential mode for the body envelope
- body phase (clickiness): adjusts the starting phase of the body. ranges from 0 to pi/2. creates a click at higher values

## group 2: pitch env settings

- pitch env attack: the attack of the pitch envelope
- pitch env release: the release of the pitch envelope. you'll want to have this around the body release or lower
- pitch env exponential envelope: enables the exponential mode for the pitch envelope
- max pitch: the maximum pitch of the pitch envelope. 16384 (4000) = the body base frequency
- min pitch: the minimum pitch of the pitch envelope. 16384 (4000) = the body base frequency

## group 3: transient settings

- transient base note: the base note for the sampled noise. 0 (80) = c5. lower values give a sample rate reduction effect
- transient attack: the attack time of the transient
- transient release: the release time of the transient
- transient exponential envelope: enables the exponential mode for the transient envelope
- transient phase: the phase (playback position) of the sampled noise

## group 4: saturation

- saturation: the input gain to the saturator. note that 0 = silence

## group 5: equalization

- eq low: the amount of low end. 256 (4000) = 0db
- eq mid: the amount of mid end. 256 (4000) = 0db
- eq high: the amount of high end. 256 (4000) = 0db

## group 6: compression

- comp threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- comp attack: the attack of the compressor in milliseconds
- comp release: the release of the compressor in milliseconds
- comp makeup gain: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db

## group 7: quality settings

- pitch quality: the sample rate of the pitch envelope. higher values give more granularity at the cost of processing power. according to nightradio, 150 hz is the sweet spot
