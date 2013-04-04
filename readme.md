Zoetrope
=====
Produce video from a bunch of frames. It takes all of the png files from the
current directory.

    zoatrope [-bpm [bpm]] [-audio [audio file]] [out file]

For example, with bpm

    zoatrope -bpm 140 fms-symphony.avi

or with an audio file

    zoatrope -audio fms-symphony.mp3 fms-symphony.avi

If you pass an audio file, the frame rate is chosen such that the frames span the
audio file.

## Bit rate calculation
From [here](http://www.videohelp.com/calc.htm)

> The basic bitrate formula is
> 
> (Size - (Audio x Length )) / Length = Video bitrate
> L = Lenght of the whole movie in seconds
> S = Size you like to use in KB (note 700 MB x 1024° = 716 800 KB) 
> A = Audio bitrate in KB/s (note 224 kbit/s = 224 / 8° = 28 KB/s)
> V = Video bitrate in KB/s, to get kbit/s multiply with 8°.
> 
> °8 bit = 1 byte.
> °1024 = 1 kilo in the computer world.
> 
> Example 
> 90 minutes video, L = 90 x 60 = 5 400 seconds
> 700 MB CD but be sure that if fits use a bit lower like 695 MB, S = 695 x 1024 = 711 680 KB
> Audio bitrate, A = 224 kbit/s / 8 = 28 KB/s
> 
> (711 680 - (5400 x 28) ) / 5400 = 104 KB/s x 8° = 830 kbit/s. 
