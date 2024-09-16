Jarvis - Personal Voice Assistant
This project is a Python-based voice assistant named Jarvis. Jarvis can perform various tasks like opening websites, fetching information from Wikipedia, sending emails, playing music, and more based on voice commands.

Features
Greeting the user: Greets based on the time of the day (Morning, Afternoon, Evening).
Wikipedia Search: Fetches and reads out summaries from Wikipedia.
Web Browsing: Opens websites like YouTube, Google, and Stack Overflow.
Play Music: Plays music from a specified directory.
Tell Time: Informs the current time.
Open Applications: Can open specific applications (e.g., Visual Studio Code).
Send Email: Sends an email via Gmail (requires SMTP configuration).
Prerequisites
To run the project, you'll need to install the following Python libraries:

In Terminal{

pip install pyttsx3
pip install speechRecognition
pip install wikipedia }
You will also need PyAudio for speech recognition:

For Windows:
Download and install the PyAudio wheel from here.
https://pypi.org/project/PyAudio/
Once downloaded, install it using:

In Terminal {
pip install <path_to_pyaudio_wheel_file> }

For macOS/Linux: 
In Terminal {
pip install pyaudio }

How to Use
Clone the repository:

Copy code
git clone https://github.com/yourusername/jarvis-assistant.git
Navigate to the project directory:

bash

cd jarvis-assistant
Install the required dependencies:

In Terminal

pip install -r requirements.txt
Update the sendEmail function with your Gmail credentials:

python

server.login('youremail@gmail.com', 'your-password')
Note: For security reasons, it's recommended to use environment variables or OAuth for authentication rather than hardcoding your credentials.

Run the script:

bash

python jarvis.py
Speak to the microphone and give commands like:

"Search Wikipedia for Python"
"Open YouTube"
"What time is it?"
"Play music"
"Send email to [name]"
Voice Commands Examples
"Search Wikipedia for Python": Fetches a short summary from Wikipedia about Python.
"Open YouTube": Opens YouTube in the web browser.
"Play music": Plays a song from the configured music directory.
"What time is it?": Tells the current time.
"Send email to [name]": Sends an email to the specified recipient.
Notes
The email-sending feature uses Gmail's SMTP. Make sure to enable "Less secure apps" in your Gmail account settings or use OAuth for secure authentication.
Customize the paths for music and application opening in the script as per your system.
Future Improvements
Adding OAuth for secure email login.
Expanding the set of voice commands.
Adding more applications and functionality based on user input.
