#abstract

a module modelling the famous clap sound from the roland tr-808

it works by retriggering a short filtered sampled noise envelope four times, with the last retrigger having a much longer envelope.
#controllers

##group 1: noise main settings

- noise transpose: the base pitch of the sampled noise in semitones. 0 (80) = c5. lower values give a sample rate reduction effect
- noise random pitch: the amount of random pitch to apply in semitones/256
- noise phase: the phase (playback position) of the noise
- noise random phase: the amount of randomness to apply to the phase

##group 2: noise filter settings

- noise filter: the type of filter to use for the sampled noise
- noise filter freq: the frequency of the filter in hertz. this is exponential if the "noise exponential filter" controller is enabled
- noise filter resonance: the resonance of the filter
- noise exponential filter: enabled exponential mode for the filter frequency

##group 3: release settings

- 1st-3rd release: the release of the first three triggers
- 4th release: the release of the fourth trigger

##group 4: delay settings

- all delay: controls the delay of all three retriggers. this overwrites the other controllers in this group
- 2nd delay: controls the delay of the second trigger
- 3rd delay: controls the delay of the third trigger
- 4th delay: controls the delay of the fourth trigger. this should be half the value of the other two for a better sound :>

##group 5: volume settings

- 1st volume: the volume of the first trigger. 128 (4000) = -6db
- 2nd volume: the volume of the second trigger. 128 (4000) = -6db
- 3rd volume: the volume of the third trigger. 128 (4000) = -6db
- 4th volume: the volume of the fourth trigger. 128 (4000) = -6db

##group 6: reverb settings

- reverb wet: the volume of the reverb (wet) signal. 128 (4000) = -6db
- reverb feedback: the feedback of the reverb
- reverb damp: the dampening (lowpass filter) of the reverb
- reverb size: the size of the reverb
- reverb seed: the random seed for the reverb