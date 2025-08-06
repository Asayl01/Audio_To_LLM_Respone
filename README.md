#  Audio To LLM Response: A Real-Time Voice Chatbot

A real-time, voice-powered chatbot that captures user speech, processes it through a Large Language Model (LLM), and responds with a generated audio reply.

---



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
