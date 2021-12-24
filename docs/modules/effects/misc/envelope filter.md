#abstract

a simple filter with an envelope triggered by a note signal

not to be confused with the traditional definition of the term, a filter with the cutoff controlled by the signal amplitude (see my wah-wah module for this, which has filter types besides bandpass)

useful as a modular synth component

no, i did not rip off logickin's module, that module has keytracking while this does not. i needed something that didn't have keytracking, hence why i made this

#controls

##group 1: filter controls

- filter freq: the exponential frequency of the filter
- filter resonance: the resonance/bandwidth of the filter
- filter gain: the gain of the filter. has a range of -24db <-> +24db
- filter type: the type of filter
- filter roll-off: the roll-off of the filter in db/oct
- filter response: the response of the filter to the envelope. 1000 (8000) is instantaneous response

##group 2: envelope main controls

- filter attack: the attack of the envelope in milliseconds
- filter decay: the decay of the envelope in milliseconds
- filter sustain: enables the envelope sustain
- filter sustain level: the sustain level of the envelope
- filter release: the release of the envelope in milliseconds

##group 3: envelope curve controls

- filter attack curve: the curve shape of the envelope attack
- filter decay curve: the curve shape of the envelope decay
- filter release curve: the curve shape of the envelope release

##group 4: envelope settings

- envelope smoothing: the type of smoothing to apply to the envelope