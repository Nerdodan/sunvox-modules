#abstract

this module was requested by neurononeuro. it is essentially an extended version of the default loop module, where the looping is gated by the note input

reset the loop by sending a note signal to this module

#controllers

##group 1: dry/wet settings

- dry: the gain of the dry signal, 128 (1000) = -6db
- wet: the gain of the wet signal, 128 (1000) = -6db

##group 2: main settings

- delay: the retrigger length of the loop in tracker lines
- channels: the channels of the loop
- repeats: the number of repeats of the loop. note that though this controller can go beyond 64, the actual loop repeat stays at 64
- mode: the mode of the loop
- loop always on: whether the loop stays on even after releasing the note