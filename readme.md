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
