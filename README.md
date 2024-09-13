# Text-to-speech-Model
A Python-based text-to-speech model using the win32com.client library, allowing users to input text and have it spoken aloud by the computer.

Features
Continuously accepts user input for conversion to speech.
Uses SAPI.SpVoice for speech synthesis.
Lightweight and easy to run on any Windows machine with Python installed.
Requirements
Windows operating system
Python 3.x installed
pywin32 package installed
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/your-username/text-to-speech-converter.git
Navigate to the project directory:

bash
Copy code
cd text-to-speech-converter
Install the required package:

bash
Copy code
pip install pywin32
Usage
Run the Python script:

bash
Copy code
python tts_converter.py
The program will continuously prompt you to input text. Once you enter the text, the computer will speak it aloud.

To exit the loop, press Ctrl+C or close the terminal.

Code Example
python
Copy code
import win32com.client

speaker = win32com.client.Dispatch("SAPI.SpVoice")

while True:
    print("Enter the word you want to be spoken aloud:")
    s = input()
    speaker.Speak(s)
License
This project is licensed under the MIT License.
