> 获取裸流
  ffmpeg -i video.mp4 -codec copy -f h264 video.h264
> gcc 
  gcc -g -Wall -o avio avio_reading.c -lavcodec -lavutil  -lavformat -lz -lm -ldl -lpthread -lrt

  -lavcodec -lavdevice -lavformat -lavutil

   编译错误问题 http://ffmpeg.org/faq.html#I_0027m-using-FFmpeg-from-within-my-C_002b_002b-application-but-the-linker-complains-about-missing-symbols-which-seem-to-be-available_002e

   $(pkg-config --cflags --libs libavformat libavcodec)


   'rtsp://10.10.32.176:554'