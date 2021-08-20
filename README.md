# Bluetooth_Audio_real-time_Play
Based on the 8311 bluetooth development board, the audio is transferred from smart phone to the board via A2DP protocol. After that the audio packets are sent to the linux OS using the uart and played in real time using the lib of SDL2
The bluetooth stack protocol project is offical and open-source. I just modify a little in /example/a2dp_sink_demo.c to let the sound card of computer play the audio in real time, while the original one save the audio data and store in the format of wav.
