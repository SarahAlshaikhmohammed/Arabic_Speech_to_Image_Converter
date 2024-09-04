
# Arabic Speech to Image Converter

This project demonstrates how to convert Arabic speech into text and then generate an image displaying the transcribed Arabic text. It uses libraries such as `speech_recognition`, `PIL`, `arabic_reshaper`, and `bidi` to achieve this.

## Features

- Converts Arabic speech from an audio file into text using Google’s Speech Recognition API.
- Processes the transcribed text to display it properly in Arabic (right-to-left).
- Generates an image with the transcribed Arabic text and saves it.

## Installation

To use this project, you need to install the required libraries. You can do so using the following commands:

```bash
pip install pydub pytube speechrecognition google-cloud-storage ffmpeg
pip install --upgrade arabic-reshaper
pip install python-bidi
```

## How to Use

1. Clone or download this repository.
2. Place the Arabic audio file that you want to transcribe in the working directory.
3. Ensure that you have an Arabic font (like IBMPlexSansArabic) for displaying the text.
4. Run the script to transcribe the audio and generate an image with the Arabic text.

### Example:

```python
# Define the path to your Arabic audio file
audio_file_path = "/path/to/audio.wav"

# Transcribe the audio file
transcribed_text = audio_to_text(audio_file_path)

# Generate an image with the transcribed Arabic text
process_text_to_image(transcribed_text)
```

In this example, the audio file `audio.wav` is transcribed into text and displayed on an image.

## License

This project is open-source and available under the MIT License.
