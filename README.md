
# Audio to LLM Response
This project is a real-time voice chatbot that captures user speech and responds with generated audio replies using an LLM.
It works by:
1. Recording the user's voice.
2. Transcribing the audio to text using Whisper.
3. Generating a response using Cohere.
4. Converting the response to audio using gTTS.
5. Playing the audio response automatically.

## Tools & Requirements

| Category      | Technology                                                                                          |
| :------------ | :-------------------------------------------------------------------------------------------------- |
| **Frontend**  | `HTML5`, `CSS3`, `Vanilla JavaScript`                                                               |
| **Backend**   | `Python 3.8+`, `Flask`, `Flask-CORS`                                                                |
| **AI & APIs** | `openai-whisper` (Speech-to-Text), `cohere` (LLM), `gTTS` (Text-to-Speech)                           |
| **Core Libs** | `Numpy`, `Scipy`                                                                                    |
| **System**    | `FFmpeg` (Required for audio processing)                                                            |
| **Dev Env**   | `Anaconda`                                                                                          |

---
## How to Run
Follow these steps to get the project running on your local machine.

### 1. Prerequisites
- Python 3.8 or newer
- FFmpeg installed and added to system PATH  
  → Download from https://ffmpeg.org/download.html

### 2. Clone or Download the Project
```bash
# If you use Git
git clone https://your-repository-url.git
cd your-project-directory
```

> Alternatively, you can download the ZIP file and extract it manually.

### 3. API Key Configuration

1. Go to [https://cohere.com](https://cohere.com) and sign up for a free account.  
   Once logged in, navigate to your dashboard and generate an API key.
2. Open the project folder and locate the `app.py` file.
3. In your code editor, find the following line:
   ```python
   COHERE_API_KEY = "YOUR_REAL_API_KEY_HERE"








```
chatbot_app/
│
├── app.py              # Main Flask server, handles all backend logic
│
├── templates/
│   └── index.html      # The HTML structure for the user interface
│
└── static/
    ├── style.css       # All CSS for styling the UI
    ├── script.js       # Frontend JavaScript for audio and API handling
    └── robot.png       # The chatbot's avatar icon
```
