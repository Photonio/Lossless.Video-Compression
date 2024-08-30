sch: https://www.google.com/search?q=h264+compress+smaller+lossless

# Discuss:
## [How to compress size lossing minum quality](https://www.reddit.com/r/handbrake/comments/13ynst2/how_to_compress_size_lossing_minum_quality/)

## [h264 lossless coding](https://stackoverflow.com/questions/6701805/h264-lossless-coding)
question:
>Is it possible to do completely lossless encoding in h264? By lossless, I mean that if I feed it a series of frames and encode them, and then if I extract all the frames from the encoded video, I will get the exact same frames as in the input, pixel by pixel, frame by frame. Is that actually possible? Take this example:

>I generate a bunch of frames, then I encode the image sequence to an uncompressed AVI (with something like virtualdub), I then apply lossless h264 (the help files claim that setting --qp 0 makes lossless compression, but I am not sure if that means that there is no loss at any point of the process or that just the quantization is lossless). I can then extract the frames from the resulting h264 video with something like mplayer.
> ...
>
>EDIT: There is a VERY valid point about lossless H264 not making too much sense. I am well aware that there is no way I could tell (with just my eyes) the difference between and uncompressed clip and another compressed at a high rate in H264, but I don't think it is not without uses. For example, it may be useful for storing video for editing without taking huge amounts of space and not losing quality and spending too much encoding time every time the file is saved.
>
>UPDATE 2: Now x264 doesn't crash. I can use as sources either avisynth or lossless yv12 lagarith (to avoid the colorspace compression warning). Howerver, even with --qp 0 and a rgb or yv12 source I still get some differences, minimal but present. This is troubling, because all the information I have found on lossless predictive coding (--qp 0) claims that the whole encoding should be lossless, but I am unable to verifiy this.

Answer:
