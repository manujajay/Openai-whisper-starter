# OpenAI-Whisper-Starter

This repository is designed to help you get started with OpenAI's Whisper, a state-of-the-art automatic speech recognition (ASR) model. It includes examples of how to use Whisper to transcribe audio files into text.

## Prerequisites

- Python 3.7 or higher
- Whisper library

## Installation

Install Whisper using pip:

```bash
pip install git+https://github.com/openai/whisper.git
```

## Basic Usage Example

### Transcribing Audio

This example demonstrates how to transcribe an audio file using Whisper.

```python
import whisper

def transcribe_audio(audio_path):
    # Load the model
    model = whisper.load_model("base")

    # Load and transcribe the audio file
    result = model.transcribe(audio_path)
    print("Transcription: ", result['text'])

# Example usage
audio_path = 'sample_audio.mp3'
transcribe_audio(audio_path)
```

## Contributing

Contributions that improve the documentation, enhance usability, or extend the functionality are welcome. Please fork the repository, create a feature branch, and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
