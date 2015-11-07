Reverberation is added to the clean signals at different approximate Reverberation Times (RT) of 0.3, 0.5 and 0.7. This is done by
generating impulse responses from many common or reasonable types in order to effectively cover the range of RTs between approximately 0.25
to 0.75.

Data is reverberated in a two stage process:

  * Generate the room impulse response for the 15 different rooms used in the database. This is done using the rir tool: http://sgm-audio.com/research/rir/rir.html
> The format for the rir command is described with the software, and basically involves providing information about 1) room dimensions,
> with the limitation that the room have only six walls, 2) impulse source location, 3) microphone position, 4) reflection coefficients
> for each of the six surfaces, ranging from 0 (least reflectivity) to 1 (greatest reflectivity). 5) speed of sound: always set to sea-level
> and is not altered in the generation of any of these impulses, 6) impulse length is always left at 2.00 seconds. 7) reverb time, peak
> impulse and echos counted are all output measures of the rir command, 8) Sample rate and sample size are always set to 8,000 Hz and 16 bits.
> The following give all the parameters needed to generate these impulse responses for each room.

1) rt0.3,a0
Long, narrow room with floor and ceiling-padded, source close to mic.

---

rm   | room dimensions | 5.00m, 18.00m, 5.00m
src  | source location | 2.50m, 2.00m, 2.50m
mic  | mic location    | 2.50m, 1.00m, 2.50m
rc   | reflection      | x0 = 0.50, x1 = 0.50
> | coefficients    | y0 = 0.60, y1 = 0.60
> |                 | z0 = 0.30, z1 = 0.30
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 3003508
> | reverb time     | 0.307 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | 0.00 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


2) rt0.5,a0
Large, moderately reflective room, low reflection floor, with mic and source in the center.

---

rm   | room dimensions | 15.00m, 18.00m, 10.00m
src  | source location | 7.50m, 9.00m, 5.00m
mic  | mic location    | 7.50m, 7.00m, 5.00m
rc   | reflection      | x0 = 0.80, x1 = 0.70
> | coefficients    | y0 = 0.80, y1 = 0.70
> |                 | z0 = 0.10, z1 = 0.70
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 500871
> | reverb time     | 0.485 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -6.02 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


3) rt0.7,a0
Medium-sized, highly reflective room, source in center at standing human mouth location, mic centered at 2 feet height next to wall.

---

rm   | room dimensions | 8.00m, 8.00m, 7.00m
src  | source location | 4.00m, 4.00m, 1.50m
mic  | mic location    | 4.00m, 0.60m, 1.00m
rc   | reflection      | x0 = 0.85, x1 = 0.85
> | coefficients    | y0 = 0.85, y1 = 0.85
> |                 | z0 = 0.70, z1 = 0.80
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 3018138
> | reverb time     | 0.677 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -10.72 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


4) rt0.3,a1
Medium sized room with low ceiling, floor padded and ceiling highly reflective, source near ceiling

---

rm   | room dimensions | 7.10m, 7.60m, 2.30m
src  | source location | 3.00m, 3.00m, 2.00m
mic  | mic location    | 3.60m, 3.20m, 1.00m
rc   | reflection      | x0 = 0.80, x1 = 0.70
> | coefficients    | y0 = 0.80, y1 = 0.80
> |                 | z0 = 0.10, z1 = 0.85
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 10895739
> | reverb time     | 0.248 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -1.46 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


5) rt0.5,a1
Long, narrow room with floor and ceiling-padded, source across the room from mic, moderately reflective surfaces


---

rm   | room dimensions | 5.00m, 18.00m, 5.00m
src  | source location | 2.50m, 17.00m, 2.50m
mic  | mic location    | 2.50m, 1.00m, 2.50m
rc   | reflection      | x0 = 0.50, x1 = 0.50
> | coefficients    | y0 = 0.60, y1 = 0.60
> |                 | z0 = 0.30, z1 = 0.30
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 3005511
> | reverb time     | 0.473 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -19.76 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


6) rt0.7,a1
Large room, moderately reverberant, microphone 15 feet from source

---

rm   | room dimensions | 20.00m, 20.00m, 5.00m
src  | source location | 6.00m, 5.00m, 1.80m
mic  | mic location    | 6.00m, 0.60m, 1.00m
rc   | reflection      | x0 = 0.70, x1 = 0.70
> | coefficients    | y0 = 0.70, y1 = 0.70
> |                 | z0 = 0.70, z1 = 0.70
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 675941
> | reverb time     | 0.700 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -13.01 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


7) rt0.3,a2
Rectangular conference room, with 12 foot padded ceiling, mic and source in opposite corners of the room.

---

rm   | room dimensions | 4.10m, 6.60m, 3.60m
src  | source location | 2.03m, 1.50m, 1.60m
mic  | mic location    | 0.60m, 5.20m, 1.40m
rc   | reflection      | x0 = 0.80, x1 = 0.80
> | coefficients    | y0 = 0.80, y1 = 0.80
> |                 | z0 = 0.50, z1 = 0.25
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 13881438
> | reverb time     | 0.319 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -11.98 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


8) rt0.5,a2
Small, highly reflective room, sourcesituated in center, mic centered at 2 feet height next to wall.

---

rm   | room dimensions | 6.00m, 6.00m, 5.00m
src  | source location | 3.00m, 3.00m, 1.50m
mic  | mic location    | 3.00m, 0.60m, 1.00m
rc   | reflection      | x0 = 0.85, x1 = 0.85
> | coefficients    | y0 = 0.85, y1 = 0.85
> |                 | z0 = 0.70, z1 = 0.80
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 7511793
> | reverb time     | 0.525 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -7.79 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


9) rt0.7,a2
Small, glass atrium, source standing in center, mic centered at 2 feet height next to wall.

---

rm   | room dimensions | 3.00m, 2.50m, 2.80m
src  | source location | 1.50m, 1.25m, 1.80m
mic  | mic location    | 1.50m, 0.60m, 1.00m
rc   | reflection      | x0 = 0.95, x1 = 0.95
> | coefficients    | y0 = 0.95, y1 = 0.85
> |                 | z0 = 0.75, z1 = 0.80
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 64387200
> | reverb time     | 0.726 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -0.26 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


10) rt0.3,a3
Medium room, source in corner across from mic, all surfaces moderately to highly reflective.

---

rm   | room dimensions | 3.00m, 5.60m, 2.90m
src  | source location | 0.33m, 0.33m, 1.60m
mic  | mic location    | 2.60m, 5.20m, 1.10m
rc   | reflection      | x0 = 0.83, x1 = 0.86
> | coefficients    | y0 = 0.72, y1 = 0.77
> |                 | z0 = 0.75, z1 = 0.79
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 27753237
> | reverb time     | 0.314 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -12.23 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


11) rt0.5,a3
Long narrow room with low reflection ceiling and floor, source centered below mic

---

rm   | room dimensions | 6.00m, 16.00m, 6.00m
src  | source location | 3.00m, 8.00m, 1.60m
mic  | mic location    | 3.00m, 3.00m, 2.00m
rc   | reflection      | x0 = 0.75, x1 = 0.65
> | coefficients    | y0 = 0.75, y1 = 0.65
> |                 | z0 = 0.20, z1 = 0.30
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 2347551
> | reverb time     | 0.482 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -14.01 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


12) rt0.7,a3
Tall room with highly reverberant floor and walls, mic centered high above source, source near floor

---

rm   | room dimensions | 6.00m, 10.00m, 22.00m
src  | source location | 3.00m, 5.00m, 0.50m
mic  | mic location    | 3.00m, 5.00m, 18.00m
rc   | reflection      | x0 = 0.85, x1 = 0.85
> | coefficients    | y0 = 0.75, y1 = 0.85
> |                 | z0 = 0.74, z1 = 0.60
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 1023962
> | reverb time     | 0.722 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -14.63 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


13) rt0.3,a4
Medium sized cubical room, source above mic close to wall, moderately reflective walls

---

rm   | room dimensions | 6.00m, 6.00m, 6.00m
src  | source location | 1.00m, 3.00m, 1.60m
mic  | mic location    | 1.00m, 1.00m, 1.60m
rc   | reflection      | x0 = 0.75, x1 = 0.80
> | coefficients    | y0 = 0.75, y1 = 0.80
> |                 | z0 = 0.70, z1 = 0.70
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 6259839
> | reverb time     | 0.323 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -6.02 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---



14) rt0.5,a4
Tall, moderately-high reverberant room, padded floor, mic offset and above source

---

rm   | room dimensions | 6.00m, 10.00m, 20.00m
src  | source location | 3.00m, 8.00m, 1.60m
mic  | mic location    | 3.00m, 3.00m, 2.00m
rc   | reflection      | x0 = 0.75, x1 = 0.85
> | coefficients    | y0 = 0.75, y1 = 0.85
> |                 | z0 = 0.20, z1 = 0.60
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 1126525
> | reverb time     | 0.493 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -13.78 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---


15) rt0.7,a4
Large rectangular room, padded ceiling and floor, source above mic at other side of room

---

rm   | room dimensions | 10.00m, 20.00m, 10.00m
src  | source location | 6.00m, 10.00m, 8.00m
mic  | mic location    | 6.00m, 2.00m, 10.00m
rc   | reflection      | x0 = 0.75, x1 = 0.75
> | coefficients    | y0 = 0.75, y1 = 0.70
> |                 | z0 = 0.30, z1 = 0.30
c    | speed of sound  | 343.0000 m/s
> | echoes counted  | 675983
> | reverb time     | 0.679 seconds (experimental)
len  | impulse length  | 2.000 seconds
norm | peak impulse    | -16.05 dB
sr   | sample rate     | 8000 Hz
bits | sample size     | 16 bits

---



  * Use the fconv tool to in the rir toolkit to convolve each reverb audio file listed in REVERB/reverb\_sessions with the corresponding room
> impulse response (according to the first subdir name in the session name).