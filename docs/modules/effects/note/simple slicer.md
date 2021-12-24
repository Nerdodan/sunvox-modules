# abstract

this module outputs phase signals to the sampler or metamodule which allow you to play certain slices of the sample/song

it's very simple in implementation, hence the name

use it to chop up your breaks (or anything really). you can also get creative with the randomization settings

# controllers

## group 1: pitch settings

- first note: the note that the first slice corresponds to. 0 = C0
- randomize: the amount of randomization of the input pitch in semitones/256

## group 2: slice settings

- slices: the number of slices
- slice offset: the offset of the slices, to be quantized
- slice qualtize: the quantization of the slicer. usually you'll want this to be one more than a multiple of the number of slices

## group 3: output transposition settings

- transpose: the transposition of the output in semitones
- finetune: the finetune of the output in semitones/256
