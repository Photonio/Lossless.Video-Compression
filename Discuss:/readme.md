sch: https://www.google.com/search?q=h264+compress+smaller+lossless

# Discuss:
## [h264 lossless coding](https://stackoverflow.com/questions/6701805/h264-lossless-coding)
question:
>Is it possible to do completely lossless encoding in h264? By lossless, I mean that if I feed it a series of frames and encode them, and then if I extract all the frames from the encoded video, I will get the exact same frames as in the input, pixel by pixel, frame by frame. Is that actually possible? Take this example:

I generate a bunch of frames, then I encode the image sequence to an uncompressed AVI (with something like virtualdub), I then apply lossless h264 (the help files claim that setting --qp 0 makes lossless compression, but I am not sure if that means that there is no loss at any point of the process or that just the quantization is lossless). I can then extract the frames from the resulting h264 video with something like mplayer.

Answer:
