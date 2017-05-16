# 编译opencv时出错
## error:
/usr/bin/ld: /usr/local/lib/libavcodec.a(avpacket.o): relocation R_X86_64_32 against `.rodata.str1.1' can not be used when making a shared object; recompile with -fPIC
/usr/local/lib/libavcodec.a: error adding symbols: Bad value

## solution:
重新配置ffmpeg
./configure --enable-nonfree --enable-pic --enable-shared
