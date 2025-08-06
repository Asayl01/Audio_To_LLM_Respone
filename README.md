
# Audio to LLM Response
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
- Requires a working microphone and internet connection

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

##  Tech Stack
This project integrates a modern set of tools for both frontend and backend development.

| Category      | Technology                                                                                          |
| :------------ | :-------------------------------------------------------------------------------------------------- |
| **Frontend**  | `HTML5`, `CSS3`, `Vanilla JavaScript`                                                               |
| **Backend**   | `Python 3.8+`, `Flask`, `Flask-CORS`                                                                |
| **AI & APIs** | `openai-whisper` (Speech-to-Text), `cohere` (LLM), `gTTS` (Text-to-Speech)                           |
| **Core Libs** | `Numpy`, `Scipy`                                                                                    |
| **System**    | `FFmpeg` (Required for audio processing)                                                            |
| **Dev Env**   | `Anaconda`                                                                                          |

---






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
