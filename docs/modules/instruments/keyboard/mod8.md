# abstract

a monophonic six-operator phase modulation/ring modulation synth inspired by native instruments fm8, image-line sytrus, and the like, based on the modulator and fmx modules

it features six main operators, each with adjustable coarse and fine detuning, waveform selection, and a repeatable adsr envelope. they can be routed to each other in a true-keytracked matrix-style router. this module also features two effect operators, x and z. x adds enveloped sampled noise and saturation, and z adds an enveloped filter. all of the operators can then be routed directly to the output

due to the 96 controller limit (which is hopefully lifted soon), some controls are limited. currently, using the controllers, only operator f can be routed to operators x and z. also, the ring modulation can only be triggered for all the connections at once. internally, the synth is capable of routing operators a - e to x and z, as well as making every individual connection different modulation types; you simply need to change the fmx module settings. also inside the module, other settings such as envelope curve types and operator feedback can be changed

capable of producing many fm and rm sounds, as well as crazy hybrids of the two

note that this module is velocity-responsive, and the volumes of the routings + op z's cutoff will change with lower velocities

this succeeds my old 4op pm module

the saturation is based on my saturator module

the filter curves were generated using pixilang. the original functions are as follows:

```
//x lp
//$y = 2 * $x

//x hp
//$y = (2 * $x) - 1

//z lp
//$y = (1 - (4 * $x)) + 1

//z bp
//$y = (1 - abs(1 - (2 * $x))) * 2

//z hp
//$y = (4 * $x) - 2
```

# controllers

## group 1: operator a controls

- op a coarse: the coarse detuning of operator a from the base pitch in semitones
- op a finetune: the fine detuning of operator a from the base pitch in semitones/256
- op a waveform: the waveform of operator a, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op a attack: the attack of operator a's envelope in milliseconds
- op a decay: the decay of operator a's envelope in milliseconds
- op a sustain: the sustain mode for operator a's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op a sustain level: the sustain level for operator a's envelope in terms of the peak level. 16384 (4000) = -12db
- op a release: the release of operator a's envelope in milliseconds

## group 2: operator b controls

- op b coarse: the coarse detuning of operator b from the base pitch in semitones
- op b finetune: the fine detuning of operator b from the base pitch in semitones/256
- op b waveform: the waveform of operator b, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op b attack: the attack of operator b's envelope in milliseconds
- op b decay: the decay of operator b's envelope in milliseconds
- op b sustain: the sustain mode for operator b's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op b sustain level: the sustain level for operator b's envelope in terms of the peak level. 16384 (4000) = -12db
- op b release: the release of operator b's envelope in milliseconds

## group 3: operator c controls

- op c coarse: the coarse detuning of operator c from the base pitch in semitones
- op c finetune: the fine detuning of operator c from the base pitch in semitones/256
- op c waveform: the waveform of operator c, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op c attack: the attack of operator c's envelope in milliseconds
- op c decay: the decay of operator c's envelope in milliseconds
- op c sustain: the sustain mode for operator c's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op c sustain level: the sustain level for operator c's envelope in terms of the peak level. 16384 (4000) = -12db
- op c release: the release of operator c's envelope in milliseconds

## group 4: operator d controls

- op d coarse: the coarse detuning of operator d from the base pitch in semitones
- op d finetune: the fine detuning of operator d from the base pitch in semitones/256
- op d waveform: the waveform of operator d, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op d attack: the attack of operator d's envelope in milliseconds
- op d decay: the decay of operator d's envelope in milliseconds
- op d sustain: the sustain mode for operator d's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op d sustain level: the sustain level for operator d's envelope in terms of the peak level. 16384 (4000) = -12db
- op d release: the release of operator d's envelope in milliseconds

## group 5: operator e controls

- op e coarse: the coarse detuning of operator e from the base pitch in semitones
- op e finetune: the fine detuning of operator e from the base pitch in semitones/256
- op e waveform: the waveform of operator e, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op e attack: the attack of operator e's envelope in milliseconds
- op e decay: the decay of operator e's envelope in milliseconds
- op e sustain: the sustain mode for operator e's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op e sustain level: the sustain level for operator e's envelope in terms of the peak level. 16384 (4000) = -12db
- op e release: the release of operator e's envelope in milliseconds

## group 6: operator f controls

- op f coarse: the coarse detuning of operator f from the base pitch in semitones
- op f finetune: the fine detuning of operator f from the base pitch in semitones/256
- op f waveform: the waveform of operator f, based on the fmx's waveforms. "custom" means this operator will use the module's audio input
- op f attack: the attack of operator f's envelope in milliseconds
- op f decay: the decay of operator f's envelope in milliseconds
- op f sustain: the sustain mode for operator f's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op f sustain level: the sustain level for operator f's envelope in terms of the peak level. 16384 (4000) = -12db
- op f release: the release of operator f's envelope in milliseconds

## group 7: operator x controls

- op x coarse: the coarse detuning of operator x from the base pitch in semitones. lower values give a comb-filtering effect
- op x finetune: the fine detuning of operator x from the base pitch in semitones/256
- op x attack: the attack of operator x's envelope in milliseconds
- op x decay: the decay of operator x's envelope in milliseconds
- op x sustain: the sustain mode for operator x's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op x sustain level: the sustain level for operator x's envelope in terms of the peak level. 16384 (4000) = -12db
- op x release: the release of operator x's envelope in milliseconds
- op x cutoff: the frequency of operator x's dual filter. 0 - 16384 (0 - 4000) correspond to the lowpass filter, and 16385 - 32768 (4001 - 8000) corresponds to the highpass filter
- op x resonance: the resonance of operator x's dual filter
- op x input gain: the input gain of operator x's saturator
- op x odd/even harmonics: the mix of operator x's symmetrical/asymmetrical saturators
- op x character: the curve shape of operator x's saturator
- op x mix: the dry/wet mix of operator x's saturation. 16384 (4000) = 50% dry 50% wet

## group 8: operator z controls

- op z attack: the attack of operator z's envelope in milliseconds
- op z decay: the decay of operator z's envelope in milliseconds
- op z sustain: the sustain mode for operator z's envelope. "repeat" means that the adr segments are repeated for the duration of the note
- op z sustain level: the sustain level for operator z's envelope in terms of the peak level. 16384 (4000) = -12db
- op z release: the release of operator z's envelope in milliseconds 
- op z mix: the filter type mixture of operator z. 0 (0) is a lowpass filter, 16384 (4000) is a bandpass filter, and 32768 (8000) is a highpass filter
- op z cutoff: the exponential frequency of operator z's filter
- op z resonance: the resonance of operator z's filter

## group 9: main operator modulation routing

- a -> b: the modulation amount between operators a and b
- a -> c: the modulation amount between operators a and c
- a -> d: the modulation amount between operators a and d
- a -> e: the modulation amount between operators a and e
- a -> f: the modulation amount between operators a and f
- b -> c: the modulation amount between operators b and c
- b -> d: the modulation amount between operators b and d
- b -> e: the modulation amount between operators b and e
- b -> f: the modulation amount between operators b and f
- c -> d: the modulation amount between operators c and d
- c -> e: the modulation amount between operators c and e
- c -> f: the modulation amount between operators c and f
- d -> e: the modulation amount between operators d and e
- d -> f: the modulation amount between operators d and f
- e -> f: the modulation amount between operators e and f

## group 10: main operator output routing

- op a out: the gain of operator a to the output. 16384 (4000) = -12db
- op b out: the gain of operator b to the output. 16384 (4000) = -12db
- op c out: the gain of operator c to the output. 16384 (4000) = -12db
- op d out: the gain of operator d to the output. 16384 (4000) = -12db
- op e out: the gain of operator e to the output. 16384 (4000) = -12db
- op f out: the gain of operator f to the output. 16384 (4000) = -12db

## group 11: effect operator routing

- f -> x: the gain of operator f to operator x. 16384 (4000) = -12db
- f -> z: the gain of operator f to operator z. 16384 (4000) = -12db
- x -> z: the gain of operator x to operator z. 16384 (4000) = -12db
- op x out: the gain of operator x to the output. 16384 (4000) = -12db
- op z out: the gain of operator z to the output. 16384 (4000) = -12db

## group 12: modulation settings

- velocity sensitivity: increases the amount of velocity sensitivity for the operators.
