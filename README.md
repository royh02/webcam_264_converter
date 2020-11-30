# webcam_264_converter
 Converts .264 files on cheap Chinese webcams to the standard .h264
 
## Credits
I was looking everywhere for a solution to my security cam's annoying .264 video files that can only be played in its proprietary player software. In comes https://spitzner.org/ and this fix is cross-platform. Thank you.

## Build
Clone this repo or download <a href="https://github.com/royh02/webcam_264_converter/blob/master/convert2.c">the C file</a> separately.
### Windows
You will need a C compiler to do this. I used <a href="https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win32/Personal%20Builds/mingw-builds/installer/mingw-w64-install.exe/download">mingdw-w64</a> for this. Just install and add **/path/to/MinGW/bin** to **PATH**\

Now, you will need to `cd` into the repo or where you downloaded the C file, and run
```
> gcc -o convert2 convert2.c
```
### Linux
Since gcc is pre-installed on most distributions, just `cd` into the repo or where you downloaded the C file and run
```
$ cc -o convert2 convert2.c
```

## Usage
With your executable file, if on **Linux**, you must make it executable first (ignore this if **Windows**)
```
$ chmod -x convert2
```
Then, to convert the 264 file,
```
$ ./convert2 /path/to/yourFile.264
```
and voila! You should be good to go!
