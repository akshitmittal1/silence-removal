# Adaptive voice activity detection

There are two features of this repository.

### vad.py

It returns the non-silent part of an audio file stitched into one audio file.

### segment.py

It returns the non-silent part of an audio file but in different files. Actually, it saves each segment of non-silent part as a different file, with its segment number and time stamp information in the saved name used for the segment.

## USAGE: 

Compress audio file by rempving silence:

`python vad.py path/to/in.wav out`

Create a bunch of audio segments separated by occurring silences, also provides the time stamps of segmented audio in terms of original audio file.

`mkdir -p out && python segment.py path/to/in.wav out/out`
