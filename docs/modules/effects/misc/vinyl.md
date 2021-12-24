#abstract

a clone of izotope's vinyl effect. it adds various sounds to the signal and performs alterations modelling the imperfections of the vinyl record

use it to make your audio sound like it's being played on a ~~toxic fume emitting~~ record (more often than not a crappy one)

#controllers

##group 1: preprocessing

- input gain: the input gain of the signal in terms of the peak value. 256 (2000) = 0db

##group 2: vinyl modelling

- age: the age of the vinyl record. when this is pushed beyone 24576 (6000), the audio becomes mono
- wear: the wear of the vinyl record.
- lofi: the digital aliasing of the vinyl record (don't question this, this was in the original plugin)

##group 3: turntable sounds

- mechanical noise volume: the gain of the mechanical noise in terms of the peak value. 256 (2000) = 0db
- electrical noise volume: the gain of the electrical noise in terms of the peak value. 256 (2000) = 0db

##group 4: vinyl dust

- dust amount: the amount of dust on the record
- dust volume: the gain of the dust in terms of the peak value. 256 (2000) = 0db

##group 5: vinyl scratches

- scratches amount: the amount of scratches on the record. note that when a scratch occurs, the audio is gated
- scratches volume: the gain of the scratches in terms of the peak value. 256 (2000) = 0db

##group 6: vinyl warp

- warp amount: the amount of warping on the record
- warp mode: the waveform of the warping