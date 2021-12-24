# abstract

an extended version of the stock compressor module

it works by sidechaining the filtered input signal to the compressor and routing a delayed signal into the main compressor input

the functionality of this module is built into my bus pro module

# controllers

## group 1: input gain

- input gain: the input gain of the signal. 256 (2000) = 0db

## group 2: sidechain processing

- lookahead: the lookahead time in milliseconds
- sidechain lp: the frequency of the 12db/oct lp filter on the sidechain signal in hertz
- sidechain hp: the frequency of the 12db/oct hp filter on the sidechain signal in hertz

## group 3: main controls

- threshold: the threshold of the compressor in terms of the peak value. 128 (2000) = -6db
- slope: the slope (ratio) of the compressor curve in percentage. 50 (2000) = 1:2
- attack: the attack of the compressor in milliseconds
- release: the release of the compressor in milliseconds
- makeup gain: the makeup gain of the compressor in terms of the peak value. 32768 (8000) = +32db
- gate: enables gate mode. in this mode, the compressor operates as a gate, inverting the compressed signal and summing it with the dry signal
- rms: enables rms mode. in this mode, the compressor uses rms (root mean square) detection

## group 4: post

- mix: the dry/wet ratio. note that 8192 (2000) = 50% wet, 100% dry and vice versa
