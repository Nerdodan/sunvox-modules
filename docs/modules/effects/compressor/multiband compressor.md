#abstract

a four-band variant of my compressor pro module

compresses each band separately and sums the bands

uses inversion-based band splits to negate phase coloration

#controllers

##group 1: band split

- band 1/2 split: the split frequency of bands 1 and 2 in hertz
- band 2/3 split: the split frequency of bands 2 and 3 in hertz
- band 3/4 split: the split frequency of bands 3 and 4 in hertz

##group 2: threshold control

- band 1 threshold: the threshold of band 1's compressor in terms of the peak value. 128 (2000) = -6db
- band 2 threshold: the threshold of band 2's compressor in terms of the peak value. 128 (2000) = -6db
- band 3 threshold: the threshold of band 3's compressor in terms of the peak value. 128 (2000) = -6db
- band 4 threshold: the threshold of band 4's compressor in terms of the peak value. 128 (2000) = -6db

##group 3: slope control

- band 1 slope: the slope (ratio) of the band 1's compressor curve in percentage. 50 (2000) = 1:2
- band 2 slope: the slope (ratio) of the band 2's compressor curve in percentage. 50 (2000) = 1:2
- band 3 slope: the slope (ratio) of the band 3's compressor curve in percentage. 50 (2000) = 1:2
- band 4 slope: the slope (ratio) of the band 4's compressor curve in percentage. 50 (2000) = 1:2

##group 4: attack control

- band 1 attack: the attack of band 1's compressor in milliseconds
- band 2 attack: the attack of band 2's compressor in milliseconds
- band 3 attack: the attack of band 3's compressor in milliseconds
- band 4 attack: the attack of band 4's compressor in milliseconds

##group 5: release control

- band 1 release: the release of band 1's compressor in milliseconds
- band 2 release: the release of band 2's compressor in milliseconds
- band 3 release: the release of band 3's compressor in milliseconds
- band 4 release: the release of band 4's compressor in milliseconds

##group 6: makeup gain control
- band 1 makeup gain: the makeup gain of band 1's compressor in terms of peak value. 1024 (8000) = +12db
- band 2 makeup gain: the makeup gain of band 2's compressor in terms of peak value. 1024 (8000) = +12db
- band 3 makeup gain: the makeup gain of band 3's compressor in terms of peak value. 1024 (8000) = +12db
- band 4 makeup gain: the makeup gain of band 4's compressor in terms of peak value. 1024 (8000) = +12db

##group 7: overall settings
- rms: enables rms mode. in this mode, each band uses rms (root mean square) detection
- lookahead: the lookahead time of each band in milliseconds. of course this applies to all bands because separate lookahead times would result in phasing