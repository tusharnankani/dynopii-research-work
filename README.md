# dynopii-research-work

## *PyVirtualAudioCable*

My understanding of a virtual audio cable: Just as there are printer drivers that do not connect to a printer at all but rather write to a PDF file.

Analogously there are virtual audio drivers available that do not connect to a physical microphone at all but can pipe input from other sources such as files or other programs.

### *Modules*

Python packages that could be used:

- **`PyAudio`**

**NOTE**: facing error while installing (*windows installation*) `pyaudio`, similar to what I faced while installing the `face_recognition` module. ([FIX](https://github.com/ageitgey/face_recognition/issues/175))

Use `pip install pipwin` and then use `pipwin install pyaudio` ([Ref](https://roytuts.com/python-voice-recording-through-microphone-for-arbitrary-time-using-pyaudio/))

- `playsound`
  - `playsound()` function plays the sound in the audio file and blocks until the file reading is completed, you can pass block=False to make the function run asynchronously.
- `pydub` (alternative to playsound - but has much more features, [pydub](https://github.com/jiaaro/pydub))
  - **`pydub`** requires **`pyaudio`** for audio playback, but with `ffmpeg` installed, it lets you play a large range of audio formats with only a few lines of code.

* **`simpleaudio`** lets you play WAV files and NumPy arrays, and gives you options to check whether a file is still playing.
* **`python-sounddevice`** and **`pyaudio`** provide bindings for the PortAudio library for cross-platform playback of WAV files

  * [python-sounddevice: device selection](https://python-sounddevice.readthedocs.io/en/0.3.7/#device-selection)
  * [python-sounddevice: Input to Output passthrough](https://python-sounddevice.readthedocs.io/en/0.4.1/examples.html#input-to-output-pass-through)
* **`winsound`** allows you to play WAV files or beep your speakers, but it works only on Windows.
---

##### xprillion mentioned `fire`

https://github.com/google/python-fire


## *References/Bibliography*

[Virtual Audio Pipeline / Blog: An overview to Virtual Audio Pipeline (sourceforge.net)](https://sourceforge.net/p/virtualaudiopip/blog/2013/06/an-overview-to-virtual-audio-pipeline/)

[How to create fake speakers and microphone in Windows 10 (technospot.net)](https://www.technospot.net/blogs/create-fake-speakers-and-mic-using-virtual-audio-cable/)

[How to enable and use virtual input devices in Windows 10 - TechRepublic](https://www.techrepublic.com/article/how-to-enable-and-use-virtual-input-devices-in-windows-10/)

[denizariyan/Real-Time-Auto-Transcriber](https://github.com/denizariyan/Real-Time-Auto-Transcriber)

[civilwargeeky/DiscordDMHelper: A discord bot utilizing discord.py, sounddevice, and VB Virtual Audio Cable to stream music from your computer to discord (github.com)](https://github.com/civilwargeeky/DiscordDMHelper)

[audio - Loopback (What u hear) recording in Python using PyAudio - Stack Overflow](https://stackoverflow.com/questions/23295920/loopback-what-u-hear-recording-in-python-using-pyaudio)

[How to Play and Record Audio in Python - Python Code (thepythoncode.com)](https://www.thepythoncode.com/article/play-and-record-audio-sound-in-python)

[Playing and Recording Sound in Python – Real Python](https://realpython.com/playing-and-recording-sound-python/)

[Python Voice Recording through Microphone for Arbitrary Time using PyAudio](https://roytuts.com/python-voice-recording-through-microphone-for-arbitrary-time-using-pyaudio/#:~:text=%20Python%20Voice%20Recording%20through%20Microphone%20for%20Arbitrary,will%20create%20a%20Python%20script%20called...%20More%20)

[Play audio as microphone input - Stack Overflow](https://stackoverflow.com/questions/20569076/play-audio-as-microphone-input)
