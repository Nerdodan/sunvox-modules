# abstract

an extension of the default drumsynth module, with two detunable drumsynths running in parallel, reverb, distortion, and compression

note that the input is not set to C5, so the sound will change if you play different keys
#controls

## group 1: drumsynth volume control

- drumsynth 1 volume: the volume of the first drumsynth unit. 128 (2000) = -6db
- drumsynth 2 volume: the volume of the second drumsynth unit. 128 (2000) = -6db

## group 2: drumsynth panning control

- drumsynth 1 panning: the panning of the first drumsynth unit. 0 (4000) = center
- drumsynth 2 panning: the panning of the second drumsynth unit. 0 (4000) = center

## group 2: drumsynth panning control

- drumsynth 1 transpose: the transposition of the first drumsynth unit. 0 (80) = the base pitch. note that this does not change the pitch of the instrument, instead it changes the drum sound selection
- drumsynth 2 transpose: the transposition of the second drumsynth unit. 0 (80) = the base pitch. note that this does not change the pitch of the instrument, instead it changes the drum sound selection

## group 3: drumsynth power control

- drumsynth 1 power: the power of the first drumsynth unit. this only affects the kick sound, it controls the body sustain amount over the length of the envelope
- drumsynth 2 power: the power of the second drumsynth unit. this only affects the kick sound, it controls the body sustain amount over the length of the envelope

## group 4: drumsynth tone control

- drumsynth 1 tone: the tone of the first drumsynth unit. this only affects the kick and snare sounds, it controls the pitch/filter frequency of the sine wave/noise
- drumsynth 2 tone: the tone of the second drumsynth unit. this only affects the kick and snare sounds, it controls the pitch/filter frequency of the sine wave/noise

## group 5: drumsynth length control

- drumsynth 1 length: the envelope length of the first drumsynth unit
- drumsynth 2 length: the envelope length of the second drumsynth unit

## group 6: reverb control

- reverb wet: the amount of the reverb (wet) signal. 128 (4000) = -6db
- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb

## group 7: distortion control

- distortion volume: the output volume of the distortion. 128 (4000) = 0db. this was necessary since the distortion can get pretty loud
- distortion type: the type of distortion
- distortion power: the power (gain) of the distortion
- distortion bits: the bit depth of the distorted signal. 16 (10) = no change to the bit depth
- distortion sample rate: the sample rate of the distorted signal in hertz
- distortion noise: the noise of the distorted signal, note that this is not the same as adding white noise, this effect adds a random value to each sample

## group 8: compression control

- compressor threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- compressor slope: the slope (ratio) of the compressor curve in percentage. 50 (2000) = 1:2
- compressor attack: the attack of the compressor in milliseconds
- compressor release: the release of the compressor in milliseconds





