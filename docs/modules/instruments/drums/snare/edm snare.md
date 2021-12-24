#abstract

a module that allows you to synthesize those huge synthetic snare drums heard in modern electronic music and electronic dance music

based on au5's great tutorial on synthesizing snares and kicks, available [here](https://www.youtube.com/watch?v=ra-mZivYchk)

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

the compression is based on my compressor pro module. note that the slope is fixed to 100 (1:infinity)

#controllers

##group 1: punch (body) settings

- punch base note: the base frequency of the body in semitones. 0 (80) = c5
- punch attack: the attack of the body. you'll want to have this at around 50-70 to make room for the transient
- punch release: the release of the body
- punch exponential envelope: enables the exponential mode for the body envelope

##group 2: pitch env settings

- pitch env attack: the attack of the pitch envelope
- pitch env release: the release of the pitch envelope. you'll want to have this around the body release or lower
- pitch env exponential envelope: enables the exponential mode for the pitch envelope
- max pitch: the maximum pitch of the pitch envelope. 16384 (4000) = the body base frequency
- min pitch: the minimum pitch of the pitch envelope. 16384 (4000) = the body base frequency

##group 3: transient settings

- transient base note: the base note for the sampled noise. 0 (80) = c5. lower values give a sample rate reduction effect
- transient attack: the attack time of the transient
- transient release: the release time of the transient
- transient exponential envelope: enables the exponential mode for the transient envelope

##group 4: tail settings

- tail attack: the attack of the tail
- tail release: the release of the tail
- tail exponential envelope: enables the exponential envelope of the tail
- tail filter: the type of filter to use for the tail
- tail filter freq: the filter frequency of the tail filter in hertz
- tail filter q: the filter resonance of the tail filter

##group 5: highpass

- hp freq: the frequency of the 48db highpass filter in hertz. you'll probably want to set this to the same frequency as the body base note
- hp q: the resonance of the 48db highpass filter

##group 6: saturation

- saturation: the input gain to the saturator. note that 0 = silence

##group 7: compression

- comp threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- comp attack: the attack of the compressor in milliseconds
- comp release: the release of the compressor in milliseconds
- comp makeup gain: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db

##group 8: reverb

- reverb wet: the volume of the reverb (wet) signal. 128 (4000) = -6db
- reverb highpass: the frequency of the 12db highpass filter on the reverb input in hertz
- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb width: the width of the reverb. 0 is mono
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb

##group 9: quality settings

- pitch quality: the sample rate of the pitch envelope. higher values give more granularity at the cost of processing power
