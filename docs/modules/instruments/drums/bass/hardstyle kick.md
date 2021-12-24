#abstract

a module that synthesizes the hard distorted kick drums heard in electronic genres like hardstyle, hardcore and speedcore

by changing the input module to 1 or 2, you can either use the built-in kick drum (based on my edm kick module) or use the module as an effect on your own drums

it works by first highpassing and saturating the intital kick sound, routing the audio to a parallel resonating bandpass filter, sending both signals to another saturator, and applying additional distortion effects via the distortion module

you can adjust the amount of the distorted signal, to get a cleaner and more impactful sound

based on some hardstyle kick tutorial on youtube, i don't remember which one it was, if you think you've found it, let me know, i think the guy was using cubase or logic

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

the equalization is based on the default eq module

the compression is based on my compressor pro module. note that the slope is fixed to 100 (1:infinity)

#controllers

##group 1: built-in kick drum controls

- body base freq: the base frequency of the body in semitones. 0 (80) = c5
- body attack: the attack of the body. you'll want to have this at around 50-70 to make room for the transient
- body release: the release of the body
- body exponential envelope: enables the exponential mode for the body envelope
- body phase (clickiness): adjusts the starting phase of the body. ranges from 0 to pi/2. creates a click at higher values
- pitch env attack: the attack of the pitch envelope
- pitch env release: the release of the pitch envelope. you'll want to have this around the body release or lower
- pitch env exponential envelope: enables the exponential mode for the pitch envelope
- max pitch: the maximum pitch of the pitch envelope. 16384 (4000) = the body base frequency
- min pitch: the minimum pitch of the pitch envelope. 16384 (4000) = the body base frequency
- transient base note: the base note for the sampled noise. 0 (80) = c5. lower values give a sample rate reduction effect
- transient attack: the attack time of the transient
- transient release: the release time of the transient
- transient exponential envelope: enables the exponential mode for the transient envelope
- transient phase: the phase (playback position) of the sampled noise
- saturation: the input gain to the saturator. note that 0 = silence
- eq low: the amount of low end. 256 (4000) = 0db
- eq mid: the amount of mid end. 256 (4000) = 0db
- eq high: the amount of high end. 256 (4000) = 0db
- threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- attack: the attack of the compressor in milliseconds
- release: the release of the compressor in milliseconds
- makeup gain: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db 

##group 2: initial highpass + saturation controls

- init highpass freq: the frequency of the highpass filter in hertz
- init highpass q: the resonance of the highpass filter
- init highpass rolloff: the roll-off of the highpass flter in db/oct
- init saturation: the input gain to the initial saturator. note that 0 = silence

##group 3: voice controls

- voice freq: the frequency of the bandpass filter in hertz. this only affects the sound if the "voice follows note pitch" controller is off
- voice q: the resonance of the bandpass filter
- voice rolloff: the roll-off of the bandpass filter in db/oct
- voice sat: the input gain to the voice saturator. note that 0 = silence

##group 4: distortion effects

- bit depth: the bit depth of the distorted signal. 16 (10) = no change to the bit depth
- freq: the sample rate of the distorted signal in hertz
- noise: the noise of the distorted signal, note that this is not the same as adding white noise, this effect adds a random value to each sample

##group 5: voice keytrack settings

- voice follows note pitch: enables keytracking for the voice
- voice pitch transpose: the transposition of the keytracking in semitones. 0 (80) = base pitch
- voice pitch finetune: the finetuning of the keytracking in semitones/256
- voice random pitch: the amount of random pitch to apply to the keytracking in semitones/256

##group 6: mix settings

- mix: the mix of the kick drum and distorted kick drum. note that 8192 (2000) = 100% dry, 50% wet and vice versa