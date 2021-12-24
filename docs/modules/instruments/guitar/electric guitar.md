# abstract

a module simulating the sound of an electric guitar/bass

it works via hybrid subtractive/physical modelling synthesis, where a pwm-modulated pulse wave is sent to an enveloped 48db lowpass filter, then a 48db highpass to simulate pinch harmonics, then an amplitude modulator, then a resonator to simulate the string, and lastly a comb filter to simulate the pickups

each string is sent to a body resonator, a high shelf to simulate pluckiness, and a set of peak filters for tone control

there are also squeaking and hum sounds built in, which can be controlled via the relevant controllers

the sound can be adjusted to simulate palm muting and pinch harmonics, as well as endless sustain for applications where the string would normally be endlessly excited, like slide guitar

the module responds to velocity, so lower velocities mean less harmonics

the sound works well by itself, though you can also send it to my cabinet or overdrive modules for cabinet and distortion pedal simulation

as of 2.0, this module uses fifo-based voice allocation

# controllers

## group 1: physical parameters

- string seed: the random seed for the string resonator
- pick position: the base pulsewidth of the oscillator, simulating the picking position
- pick hardness: the gain of the high shelf filter, simulating the picking hardness
- pickup position: the comb filter frequency, simulating the pickup position. this only simulates a single pickup
- body seed: the random seed for the body resonator

## group 2: squeak parameters

- squeak: the squeak trigger and length. the squeak is not triggered by a note, but rather by automating this paramater. higher values make the squeak longer
- squeak volume: the volume in terms of the peak level and filter frequency of the squeak. 16384 (4000) = -6db
- squeak seed: the random seed of the squeak resonator

## group 3: hum parameters

- hum volume: the volume of the hum in terms of the peak level. 16384 (4000) = -6db

## group 4: tone control

- bass tone: the gain of the bass peak. set to 70 hertz
- mid tone: the gain of the mid peak. set to 503 hertz
- treble tone: the gain of the treble peak. set to 6308 hertz

## group 5: playing parameters

- mute amount: the amount of palm muting
- pinch amount: the amount of pinch harmonics
- sustain mode: enables sustain for the string envelopes
- sustain amount: the sustain level for the string envelopes

## group 6: sound2ctl sample rate settings

- envelope sample rate: the sample rate of the sound2ctl modules in hertz. requested by nightradio. increasing this increases the granularity at the cost of processing power. according to nr, 150 hz is the sweet spot

