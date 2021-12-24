# abstract

a clone of the ott preset from ableton live's multiband dynamics effect, widely used in electronic dance music and made into a plugin by xfer records

it works by splitting the audio into three bands, applying heavy upwards and downwards compression to each band, and summing the bands together with optional equalization

use it to make your basses (or anything really) more biting and squashed

this module's controls are based on xfer's plugin

note that this does not use inversion-based splitting, true to the original effect. i can make an inversion based one if people want me to

# controllers

## group 1: main controls

- depth: the amount (dry/wet) of the effect
- time: the attack/release of the compressors. 4096 (1000) = 13ms/132ms on the highs, 22ms/282ms on the mids, and 48ms/282ms on the lows
- in gain: the input gain of the compressors. 8192 (2000) = 0db
- out gain: the output gain of the compressors. 8192 (2000) = 0db

## group 2: threshold controls

- h threshold: the threshold of the high compressor pair. 16384 (4000) = -35.5db downward, -40.8db upward
- m threshold: the threshold of the mid compressor pair. 16384 (4000) = -30.2db downward, -41.8db upward
- l threshold: the threshold of the low compressor pair. 16384 (4000) = -33.8db downward, -40.8db upward

## group 3: equalization controls

- h: gain of the high band. 256 (2000) = 0db
- m: gain of the mid band. 256 (2000) = 0db
- l: gain of the low band. 256 (2000) = 0db

## group 4: compression amount controls
- upwd: slope (ratio) of the upward compressors. 32768 (8000) = 200%
- dnwd: slope (ratio) of the downward compressors. 32768 (8000) = 200%
