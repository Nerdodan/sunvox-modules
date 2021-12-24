#abstract

this is a module that contains volume, balance, and stereo width control, as well as haas delay, saturation, and compression. as the name implies, it is intended to be used for bus/mix processing

the waveshaper curves were generated using pixilang, i'll see if i can find the original file

#controllers

##group 1: main processing

- volume: the volume of the signal in terms of the peak level. 16384 (4000) = -6db
- balance: the stereo balance of the signal
- position: the haas delay of the signal. moving the value left or right from the center will make the audio appear to come from the left or right less artificially than standard panning. 16384 (4000) = no delay
- stereo width: the stereo width of the signal

##group 2: highpass filter

- hp freq: the frequency of the highpass filter in hertz
- hp q: the resonance of the highpass filter
- hp roll-off: the roll-off of the highpass filter in db/oct
- hp mix: the dry/wet mixture of the highpass filter. 16384 (4000) = 50% dry 50% wet

##group 2: lowpass filter

- lp freq: the frequency of the lowpass filter in hertz
- lp q: the resonance of the lowpass filter
- lp roll-off: the roll-off of the lowpass filter in db/oct
- lp mix: the dry/wet mixture of the lowpass filter. 16384 (4000) = 50% dry 50% wet

##group 3: saturation

- saturator input gain: the input gain of the signal in terms of the peak value. 256 (2000) = 0db
- saturator odd/even harmonics: the mix of the symmetrical/asymmetrical saturators
- saturator character: the curve shape of the saturator
- saturator mix: the dry/wet mix of the saturation. 16384 (4000) = 50% dry 50% wet

##group 4: compression

- compressor input gain: the input gain of the signal. 256 (2000) = 0db
- compressor lookahead: the lookahead time in milliseconds
- compressor threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- compressor slope: the slope (ratio) of the compressor curve in percentage. 50 (2000) = 1:2
- compressor attack: the attack of the compressor in milliseconds
- compressor release: the release of the compressor in milliseconds
- compressor makeup gain: the makeup gain of the compressor in terms of peak value. 32768 (8000) = +32db
- compressor gate: enables gate mode. in this mode, the compressor operates as a gate, inverting the compressed signal and summing it with the dry signal
- compressor rms: enables rms mode. in this mode, the compressor uses rms (root mean square) detection
- compressor mix: the dry/wet ratio. note that 8192 (2000) = 50% wet, 100% dry and vice versa



