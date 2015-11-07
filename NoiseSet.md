The following are the steps to create the noisy wavs used for trials and trainining.

  * Convert the waveforms listed in file NOISE/clean\_sessions.all from whatever format you have them on (or as released by NIST) to raw format. Place them  in local dirs mix10 and mix08 such that the file NOISE/clean\_sessions.all corresponds to the relative paths to those raw waveforms.

  * Then, do the noise addition using the following code:

foreach N (B01 B02 B03 B04 B05 B06 B07 B08 A09 A10 A11 A12 A13 A14 A15)

> foreach SNR ( 08 15 20 )

> filter\_add\_noise -d -f g712 -n $DIR/NOISE/noise\_wavs/noise$N -i $DIR/NOISE/clean\_sessions.$N -o $DIR/NOISE/noisy\_sessions.$N.$SNR -s $SNR -e log.$N.$SNR -a $DIR/NOISE/start\_times.$N

> end

end

where DIR is the directory where you placed the prism evalset package and the filter\_add\_noise is a script that is part of the FaNT package (http://dnt.kr.hs-niederrhein.de/download.html).

  * This will create noisy raw wavs which you will need to convert to whichever format you need.


Note: The noisy waveforms were obtained from freesound.org and cleaned to remove single-speaker foreground speech sounds and artifacts. Only half of the original waveform is used for each of our noises (this was done doing research to keep a held-out part of the noisy waveform for training, but this held-out half is currently not being used). Finally, the chosen half is repeated to reach a length that would cover the longest waveform that needs to be distorted.

This is where the different samples come from:

our\_name  freesound\_user waveform

noiseB01  lonemonk       Approx\_5000\_Crowd\_Noise

noiseB02  Bram           01\_barcelona\_bcn\_airport\_gate39\_announcement

noiseB03  LG             Office01

noiseB04  fogma          Bar\_atmosphere\_Not\_So\_Busy

noiseB05  patchen        frost\_lobby2

noiseB06  sagetyrtle     freemall

noiseB07  pete668        AIRP0RT-CHILDREN

noiseB08  Therac\_25      galleria\_food\_court\_lunch\_15min

noiseA09  inchadney      IKEA\_Cafeteria

noiseA10  sagetyrtle     foodcourt

noiseA11  digifishmusic  IKEA\_Cafeteria

noiseA12  Robinhood76    00701\_men\_crowd\_2

noiseA13  joedeshon      church\_wedding\_ambiance\_01

noiseA14  shazam118      audience

noiseA15  joly1          cocktail\_amb\_DEF