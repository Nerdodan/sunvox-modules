#abstract

this is a module that contains volume, balance, and stereo width control, as well as haas delay. as the name implies, it is intended to be used for bus/mix processing

for more functionality, including saturation and compression, please see my bus pro module

#controllers

##group 1: main processing

- volume: the volume of the signal in terms of the peak level. 16384 (4000) = -6db
- balance: the stereo balance of the signal
- position: the haas delay of the signal. moving the value left or right from the center will make the audio appear to come from the left or right less artificially than standard panning. 16384 (4000) = no delay
- stereo width: the stereo width of the signal