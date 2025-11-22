# **🎵 Glitch-Fi Converter 🎵**

A simple, powerful command-line utility for macOS to "corrupt" and remix any audio file into a **Glitch-Fi / Data-Drift** track.  
This script takes your input MP3 and applies a unique effects chain to make it sound like a forgotten memory on a corrupted hard drive—nostalgic, chill, and broken.  
It's the perfect tool for creating unique soundscapes for TikTok, YouTube, or just for fun.

## **What It Does**

The glitchify.sh script is a filter chain that uses **FFmpeg** and **SoX** to apply a series of "Glitch-Fi" effects to your track:

1. **Downsamples:** Instantly "degrades" the audio for a crunchy, lo-fi sound.  
2. **Bandpass Filter:** Cuts the deep bass and high treble, giving it a "telephone" or "old radio" vibe.  
3. **Tape Warble:** Adds a subtle pitch wobble to mimic a warped cassette.  
4. **Atmospheric Reverb:** Drenches the track in a vast, dreamy "Slushwave" reverb.  
5. **Digital Overdrive:** Adds a bit of gritty "Phonk" distortion.  
6. **Stutter/Glitch:** Repeats a tiny slice of audio to create a signature "data-drift" glitch.

## **🛠️ Installation (macOS)**

This script relies on two powerful (and free) command-line tools: **FFmpeg** and **SoX**.

1. **Install Homebrew:** If you don't have it, open your Terminal and paste:  
   /bin/bash \-c "$(curl \-fsSL \[https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh\](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh))"

2. **Install FFmpeg and SoX:**  
   brew install ffmpeg sox

3. **Clone this Repository:**  
   git clone \[https://github.com/frangedev/glitchify.git\](https://github.com/frangedev/glitchify.git)  
   cd glitchify

4. **Make the Script Executable:**  
   chmod \+x glitchify.sh

## **🚀 How to Use**

Using the script is simple. Just pass an MP3 file to it as an argument.  
./glitchify.sh "/path/to/your/song.mp3"

**Example:**  
./glitchify.sh my\_new\_beat.mp3

The script will run and output a new file in the same directory, prefixed with glitched\_.  
Output:  
glitched\_my\_new\_beat.mp3

## **💡 Future Ideas & Contributing**

This is just the beginning. Pull Requests are welcome\! Here are some ideas to make this tool even better:

* **🎛️ Modes:** Add flags for different preset vibes:  
  * ./glitchify.sh \--mode=dark (more distortion, less reverb)  
  * ./glitchify.sh \--mode=dreamy (heavy reverb, more warble)  
* **🎲 Randomization:** Add random values for the vibrato or repeat effects so every conversion is unique.  
* **🎞️ Texture Mixing:** Add a feature to randomly mix in a background texture (like vinyl\_crackle.wav or data\_noise.wav) from a textures/ folder.  
* **🖼️ Video:** Add an option to take the new MP3 and loop it over a static image or GIF to create a simple video file, ready for YouTube.

## **License**

This project is licensed under the MIT License \- see the [LICENSE.md](http://docs.google.com/LICENSE.md) file for details.
