# Audio_To_LLM_Response

This project is a real-time voice chatbot that captures user speech and responds with generated audio replies using an LLM.

It works by:
1. Recording the user's voice.
2. Transcribing the audio to text using Whisper.
3. Generating a response using Cohere.
4. Converting the response to audio using gTTS.
5. Playing the audio response automatically.

## Tools & Requirements
- Frontend: HTML, CSS, JavaScript (vanilla)
- Backend: Python 3.8+, Flask, Flask-CORS
- Libraries: openai-whisper, cohere, gTTS, FFmpeg
- Environment: Developed and tested using Anaconda

##  How to Run

Follow these steps to get the project running on your local machine.

### 1. Prerequisites

-   Ensure you have **Python 3.8** or newer installed.
-   Ensure **FFmpeg** is installed on your system and accessible from the command line. You can download it from the [official website](https://ffmpeg.org/download.html ) and add it to your system's PATH.

### 2. Clone or Download the Project

```bash
# If you use Git
git clone https://your-repository-url.git
cd your-project-directory
```
Alternatively, download the source code and extract it into a folder.

### 3. Install Dependencies

Open a terminal or `Anaconda Prompt` in the project's root directory and run the following command to install all required Python libraries:

```bash
pip install Flask Flask-CORS openai-whisper cohere numpy scipy
```

### 4. Add API Key

1.  Go to the [Cohere website](https://cohere.com/ ), sign up for a free account, and get your API key.
2.  Open the `app.py` file.
3.  Find the following line:
    ```python
    COHERE_API_KEY = "YOUR_REAL_API_KEY_HERE"
    ```
4.  Replace `"YOUR_REAL_API_KEY_HERE"` with your actual Cohere API key.

### 5. Run the Server

In the same terminal, run the Flask server:

```bash
python app.py
```

### 6. Open the Application

1.  After running the server, you will see a message indicating that it's running on `http://127.0.0.1:5000`.
2.  Open your web browser and navigate to this address:
    [http://127.0.0.1:5000](http://127.0.0.1:5000 )
3.  Allow the browser to use your microphone when prompted.
4.  Click the microphone button and start talking!

##  Project Structure

```
chatbot_app/
│
├── app.py              # Flask server and all backend logic
│
├── templates/
│   └── index.html      # The main HTML structure of the web page
│
└── static/
    ├── style.css       # All CSS styling
    ├── script.js       # Frontend logic (audio recording, API calls)
    └── robot.png       # The bot's icon
```
---
