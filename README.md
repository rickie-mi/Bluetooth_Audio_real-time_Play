# Bluetooth_Audio_real-time_Play
Based on the 8311 bluetooth development board, the audio is transferred from smart phone to the board via A2DP protocol. After that the audio packets are sent to the linux OS using the uart and played in real time using the lib of SDL2.

The bluetooth stack protocol project is offical and open-source. I just modify a little in the file of the path(/example/a2dp_sink_demo.c) to let the sound card of computer play the audio in real time, while the original one save the audio data and store in the format of wav.

To start with, the package of SDL2 should be installed. SDL2, which provides several functions for controlling images, sounds, and I/O, allowing developers to develop application software across multiple platforms (Linux, Windows, Mac OS X, etc.) as long as they use the same or similar code. The detail of the installation can be referred from https://blog.csdn.net/qq_40017011/article/details/119748492

After installation, the content in /example/Makefile.inc should be modified to include the SDL libs, don't forget that. 

Then you can make the project in the /port/posix_h4 and check whether the audio can be played in real time.
