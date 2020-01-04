# FFmpeg
This script is made to compile FFmpeg with common codecs on Linux and Mac OSX.

## Result
This repository builds ffmpeg, ffprobe and ffserver for Mac OSX and Linux using
- build tools
    - [nasm](http://www.nasm.us/)
- video codecs
    - [x264](http://www.videolan.org/developers/x264.html) for H.264 encoding
- audio codecs
    - [LAME](http://lame.sourceforge.net/) for MP3 encoding

## Execution
To run this script simply execute the build.sh script.
```
./build.sh
```

## Folder Structure
All files that are downloaded and generated through this script are placed in the current working directory. The recommendation is to use an empty folder for this.
```
mkdir ffmpeg-compile
cd ffmpeg-compile
```

Now execute the script using:
```
../path/to/repository/build.sh
```

After the execution a new folder called "out" exists. It contains the compiled FFmpeg binary (in the bin sub-folder).
The ffmpeg-success.zip contains also all binary files of FFmpeg.

## Build failed?
Check the detailed logfiles in the working directory. Each build step has its own file starting with "build-*".