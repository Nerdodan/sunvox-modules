# abstract

this is a module that harmonizes the note input based on the diatonic (major) scale. black notes are not accepted, so you'll have to use an external multisynth to transpose to different scales

this lite version eschews amplifier/sound2ctl switches and instead uses a square multictl curve, which is significantly lighter on the cpu

along with simply playing a chord with one note, you could also randomly automate the controllers for a generative chord sequence :)

# controllers

## group 1: chord tones enable

- enable root: enables the root of the chord
- enable third: enables the third of the chord
- enable fifth: enables the fifth of the chord
- enable seventh: enables the seventh of the chord

## group 2: octave doubling settings

- enable upper root double: enables the upper octave root double
- enable lower root double: enables the lower octave root double
- enable upper third double: enables the upper octave third double
- enable lower third double: enables the lower octave third double
- enable upper fifth double: enables the upper octave fifth double
- enable lower fifth double: enables the lower octave fifth double
- enable upper seventh double: enables the upper octave seventh double
- enable lower seventh double: enables the lower octave seventh double

## group 3: inversion settings

- 1st inversion: transposes the root + doubles up one octave
- 2nd inversion: transposes the third + doubles up one octave
- 3rd inversion: transposes the fifth + doubles up one octave
- 4th inversion: transposes the seventh + doubles up one octave
