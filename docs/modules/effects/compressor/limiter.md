# abstract

a digital peak limiter

uses two limiting stages, with one having lookahead and adjustable attack and release, and the other having only release and zero attack

# controllers

## group 1: input gain

- input gain: the input gain of the signal in terms of peak value. 256 (2000) = 0db

## group 2: lookahead limiter settings

- threshold: the threshold of the limiter stage in terms of the peak value. 128 (2000) = -6db
- attack: the attack of the lookahead limiter stage in milliseconds
- release: the release of the lookahead limiter stage in milliseconds
- lookahead time: the lookahead time of the lookahead limiter stage in milliseconds

## group 3: brickwall limiter settings

- threshold: the threshold of the brickwall limiter stage in terms of the peak value. 128 (2000) = -6db
- release: the release of the brickwall limiter stage in milliseconds