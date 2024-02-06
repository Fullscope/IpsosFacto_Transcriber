# Whisper in combination with GPT-3 and Streamlit 

Upload a audio file to generate a transcript using OpenAI WHisper
## Installation:
* Setup a VirtualEnvironment or Simply run the command ***pip install -r requirements.txt*** to install the necessary dependencies.
* Make sure you check requirements.txt for the latest version of the dependencies.
* Make sure you have the following installed:
ffmpeg
rust (for tiktoken)
gcloud(for google storage)
* setup your db info and openai API keys, in a file called database.ini
* setup your google storage keys in a file called google_storage.json

## Usage:

1. Simply run the command: 
```
streamlit run app.py
```
2. Navigate to http://localhost:8501 in your web-browser.