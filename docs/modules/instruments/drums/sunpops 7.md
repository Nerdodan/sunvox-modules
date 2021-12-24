# abstract

a sunvox clone of the korg minipops 7 drum machine, famously used by jean-michel jarre and others

the way it worked was you could push in buttons and it would play back various drum patterns. you could push in multiple buttons and you could get interesting rhythm combinations

here, the buttons are notes, with the leftmost button being c0 and the last button being a0 before cycling around again. simply push in a note to get a pattern. you can push multiple notes to layer different patterns. you can also flip the "rhythm section switch" controller to access the other set of patterns

the patterns are as follows:

- c0: waltz/jazz waltz
- c#0: samba/conga
- d0: mambo/cha-cha
- d#0: rumba/beguine
- e0: tango/habanera
- f0: bossanova/slow rock
- f#0: rock 1/rock 2
- g0: rock 3/rock 4
- g#0: march 2/4/march 6/8
- a0: swing/latin swing

i did a lot of research and tried to replicate the original machine's behavior, and i'd say everything mostly works well except for layering the waltz with the other patterns. but, that's relatively minor.

use this for recreating those classic 70's synth rhythms. this also works well as a quick way to get nice foley loops. the special thing about this is that while the original synth was basically a black box, this metamodule allows you to go inside and modify the sequences and instruments.

# controllers

## group 1: instrument volume settings

- quijada: the volume of the quijada instrument in terms of the peak level. 16384 (4000) = -6db
- guiro: the volume of the guiro instrument in terms of the peak level. 16384 (4000) = -6db
- tambourine: the volume of the tambourine instrument in terms of the peak level. 16384 (4000) = -6db

## group 2: main settings

- volume: the overall volume in terms of the peak level. 16384 (4000) = -6db
- balance: the volume of the cymbals in terms of the peak level. 16384 (4000) = -6db
- tempo: the tempo of the machine. ranges linearly from 32 bpm to 256 bpm

## group 3: rhythm section settings

- rhythm section switch: enables the second set of patterns. the pattern will not switch until the current set of measures in the pattern is complete
