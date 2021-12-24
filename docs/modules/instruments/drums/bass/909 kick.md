# abstract

a simple clone of the kick drum from the roland tr-909. it works simply by generating a low tone with a pitch envelope and some mild saturation

for an updated and more generalized version of this module, please see my analog kick module

the saturation is based on my saturator module's hard odd curve, which was generated in pixilang. i'll see if i can find the original file

# controllers

## group 1: body controls

- body max tone: the maximum tone of the pitch envelope. 16384 (4000) = c5
- body min tone: the minimum tone of the pitch envelope. 16384 (4000) = c5
- body phase: the starting phase of the tone. 8192 (2000) = pi/2
- body release: the release time of the tone

## group 2: pitch env controls

- pitch env release: the release of the pitch envelope

## group 3: saturation controls

- saturation: the input gain to the saturator. note that 0 = silence