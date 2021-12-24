# abstract

an analog string ensemble synth inspired by the eminent 3310, used by jean-michel jarre and others

it simply uses two sawtooth oscillators, one detuned an octave above the other, with additonal chorus

unlike the original, this also includes an asr envelope, echo, and phaser effects

perfect for those spacey 70's synth string sounds

# controllers

##group 1: upper octave controls

- upper octave volume: the volume of the upper octave oscillator in terms of the peak level. 128 (4000) = -6db

## group 2: envelope controls

- attack: the attack of the amplitude envelope
- release: the release of the amplitude envelope
- sustain: enables the sustain of the amplitude envelope

## group 3: chorus controls

- chorus mix: the amount of chorus (wet) signal in terms of the peak level. 16384 (4000) = -6db
- chorus depth: the depth of the chorus
- chorus freq: the speed of the chorus

## group 4: echo controls

- echo wet: the amount of echo (wet) signal in terms of the peak level. 128 (4000) = -6db
- echo feedback: the feedback of the echo
- echo delay: the delay of the echo in seconds/256. maximum delay is 2 seconds
- echo right channel offset: whether to offset the right channel by half the echo delay

## group 5: phaser controls

- phaser wet: the amount of phaser (wet) signal in terms of the peak level. 16384 (4000) = -6db
- phaser freq: the frequency of the allpass filter in hertz
- phaser q: the resonance of the allpass filter in hertz
- phaser lfo freq: the frequency of the allpass filter frequency lfo in the chosen frequency unit
- phaser lfo amp: the amplitude of the allpass filter frequency lfo
- phaser lfo wave: the waveform of the allpass filter frequency lfo
- phaser lfo unit: the frequency unit for the allpass filter frequency lfo