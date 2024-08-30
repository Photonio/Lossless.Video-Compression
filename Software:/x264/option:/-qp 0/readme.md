sch: https://www.google.com/search?q=x264+-qp+0

# Doc:
https://trac.ffmpeg.org/wiki/Encode/H.2642

# Discuss:
Answer: 1
- https://stackoverflow.com/questions/6701805/h264-lossless-coding/12303936
>FFmpeg has a "lossless" mode for x264, see FFmpeg and x264 Encoding Guide
>
>§ Lossless H.264
>in essence it's -qp 0

Answer: 2
- https://stackoverflow.com/questions/6701805/h264-lossless-coding/8921022
>For encoding lossless RGB with x264, you should use the command line version of x264 (you can't trust GUIs in this edge case, they will probably mess-up) r2020 or newer, with something like that:
>
>`x264 --qp 0 --preset fast --input-csp rgb --output-csp rgb --colormatrix GBR --output "the_lossless_output.mkv" "someinput.avs"`
>
>Any losses/differences between the input and output should be from some colour space conversion (either before encoding, or at playback), wrong settings or some header/meta-data that was lost. x264 don't supports RGBA, but RGB is ok. YUV 4:4:4 compression is more efficient, but you will lose some data in colour space conversion as your input is RGB. YV12/i420 is much smaller, and by far the most common colour space in video, but you have less chroma resolution.
>
>More information on x264 settings: http://mewiki.project357.com/wiki/X264_Settings
>
>Also, avoid lagarith. It uses x87 floating point... and there are better alternatives. http://codecs.multimedia.cx/?p=303 http://mod16.org/hurfdurf/?p=142
