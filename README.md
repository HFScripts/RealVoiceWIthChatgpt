- This code is a Python script that uses the SpeechRecognition library to listen for audio input from a microphone, and sends the speech to the OpenAI GPT-3 language model for processing. If the user says "ask AI" followed by a phrase, the script will send the phrase to the OpenAI model and receive a response. The response is then converted to an MP3 file using the Eleven Labs API text-to-speech service, which is played back using the Pygame library.

## SETUP INSTRUCTIONS

### Install Anaconda:
Anaconda is a package manager for Python that includes many useful libraries and tools. It also provides a convenient way to manage Python environments. You can download the Anaconda installer from the official website: https://www.anaconda.com/products/individual

### Add pygame via conda-forge:
To install the Pygame library, you can use the conda-forge channel. Open a terminal or Anaconda prompt and type the following command:

```conda install -c conda-forge pygame```

### Create a new environment:
To create a new environment called "py39voice" with Python version 3.9, you can use the following command:

```conda create -n py39voice python=3.9```

### Activate the environment:
To activate the "py39voice" environment, type the following command:

```conda activate py39voice```

### Install required packages:
The following packages are required for this script to run:

- SpeechRecognition
- OpenAI
- requests
- Pygame

#### You can install them using the following command:

```pip install SpeechRecognition openai requests pygame```

## USAGE

To run the script, activate the "py39voice" environment and run the following command:

```python voice_ai.py```

The script will continuously listen for audio input from the microphone. When the user says "ask AI" followed by a phrase, the script will send the phrase to the OpenAI model and play back the response as an MP3 file. The Pygame mixer will automatically open and close, and the MP3 file will be deleted after playback. To stop the script, press Ctrl+C in the terminal.
