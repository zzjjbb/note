# Build FFmpeg

## Minimum build for RTMP streaming

```bash
curl -sSL https://ffmpeg.org/releases/ffmpeg-5.0.1.tar.gz -o ffmpeg.tar.gz
tar -xvf ffmpeg.tar.gz
cd ffmpeg-5.0.1
./configure --disable-w32threads --disable-os2threads --disable-alsa --disable-appkit --disable-avfoundation --disable-bzlib \
--disable-coreimage --disable-iconv --disable-libxcb --disable-libxcb-shm --disable-libxcb-xfixes --disable-libxcb-shape \
--disable-lzma --disable-sndio --disable-sdl2 --disable-xlib --disable-zlib --disable-amf --disable-audiotoolbox --disable-cuda \
--disable-cuvid --disable-d3d11va --disable-dxva2 --disable-nvdec --disable-nvenc \
--disable-v4l2-m2m --disable-vaapi --disable-vdpau --disable-videotoolbox --disable-everything \
--enable-demuxer=flv,mov,mpegts,live_flv --enable-muxer=flv,mov,mpegts --enable-protocol=file,rtmp,pipe,rtmps \
--enable-bsf=aac_adtstoasc,h264_mp4toannexb \
--disable-avdevice --disable-swscale --disable-postproc --disable-doc --disable-runtime-cpudetect \
--enable-openssl --enable-pthreads --enable-version3 --enable-avcodec --enable-avformat --enable-swresample --enable-avfilter \
--disable-programs --enable-ffmpeg --enable-small
# make -j4
# mv ffmpeg ..
```

