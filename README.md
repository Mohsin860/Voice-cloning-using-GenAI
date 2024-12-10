

# Voice Cloning Project

This project demonstrates how to clone a speaker's voice and use it to generate speech from text. It uses two powerful tools:

1. **SpeechBrain**: For extracting speaker embeddings (which capture the unique features of a person’s voice).
2. **Microsoft’s SpeechT5**: For generating speech using the extracted voice features and given text.

## What This Project Does:

1. **Extracts Speaker Embedding**: 
   - This step captures the unique characteristics of a person's voice from a reference audio file (like a recording of them speaking).
  
2. **Synthesizes Speech**: 
   - Using the extracted voice features, the system generates speech that sounds like the original speaker, but with new text.

## How It Works:

1. **Step 1**: Upload a reference audio file where the speaker says something.
2. **Step 2**: The script extracts the speaker's voice features from the file.
3. **Step 3**: You provide some text, and the system generates speech in the same voice from the reference audio.

## Prerequisites:

Before running this project, make sure you have the following installed:

- **Python 3.x** (preferably Python 3.7 or above)
- **PyTorch**: For machine learning model operations.
- **Torchaudio**: For handling audio files.
- **Transformers**: For text-to-speech generation.
- **SpeechBrain**: For extracting speaker embeddings.
- **Soundfile**: For saving the synthesized audio.

## Setup:

1. **Clone this repository** to your local machine:

   ```bash
   git clone https://github.com/your-username/voice-cloning.git
   ```

2. **Install required libraries**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the necessary models**:
   - When you run the script for the first time, the models will be automatically downloaded. Make sure you have a stable internet connection.

## Usage:

1. **Provide a Reference Audio**:
   - Prepare a reference audio file of the speaker's voice (e.g., "me.wav"). This file will be used to extract the voice features.

2. **Run the Script**:
   - Once the environment is set up, run the `main.py` file:

   ```bash
   python main.py
   ```

3. **Text-to-Speech**:
   - The script will generate speech using the voice extracted from the reference audio and will save the synthesized speech to a `.wav` file.

4. **Check the Output**:
   - The synthesized speech will be saved as `synthesized_speech.wav`. You can change the output file name in the script if needed.

## Example:

- Input Texts:
   - "My name is Mohsin, and I have completed sixteen years of education."
   - "This is a demonstration of voice cloning technology."

- Output: The synthesized audio will sound like the speaker from the provided reference audio, saying the input texts.

## Troubleshooting:

- **Audio Quality**: The quality of the generated speech depends on the clarity and length of the reference audio.
- **Model Downloads**: Ensure you have a stable internet connection as the models are large and need to be downloaded.

