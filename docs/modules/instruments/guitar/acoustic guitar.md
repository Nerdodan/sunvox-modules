# abstract

a module roughly simulating the sound of an acoustic guitar/bass. it uses a custom waveform with a keytracked filter frequency and release, sent to a high shelf filter to simulate the pluckiness amount, then sent to two parallel resonator units, one inverted, to simulate the body of the instrument

the drawn waveform was provided by so?ing machine (aka saltbearer)

# controllers

## group 1: main parameters

- pluckiness: the amount of high shelf gain on the oscillator
- release: the release (muting) of the oscillator

## group 2: resonator parameters

- reverb seed: the random seed for the resonator
- inverse reverb seed: the random seed for the inverse resonator