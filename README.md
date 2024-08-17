# Speech-To-Text
Convertion of spoken words into text.

This project involves the following steps:

Step 1: Libraries
- speech_recognition
- AudioSegment from pydub
- requests
- os

Step 2: Function to download the audio file from a URL
- A URL as input
- An HTTP GET request to download the audio file
- Store it in memory using a BytesIO object
- Return the audio data, if download success. Otherwise, raise an exception.

Step 3: Function to convert the audio from MP3 to WAV
- Convert an MP3 file to WAV format
- Use pydub's AudioSegment to read the MP3 data
- Export it as a WAV file
- Store the WAV data in a BytesIO object.

Step 4: Function to transcribe audio file using CMU Sphinx
- Create a Recognizer object
- Read the audio file into memory
- Try to recognize the speech:
- If successful, return the transcribed text. If not, handle errors and return appropriate messages.

Step 5: Execution
- Specify the URL of the MP3 file to be downloaded.
- Download the audio file.
- If successful, convert the MP3 to WAV.
- If the conversion is successful, transcribe the audio
- Print the resulting text.
