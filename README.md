#  Audio To LLM Response: A Real-Time Voice Chatbot

[![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue.svg )](https://www.python.org/downloads/ )
[![Flask](https://img.shields.io/badge/Flask-2.x-black.svg )](https://flask.palletsprojects.com/ )
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg )](https://opensource.org/licenses/MIT )

A real-time, voice-powered chatbot that captures user speech, processes it through a Large Language Model (LLM), and responds with a generated audio reply.

---

##  Core Functionality

The application operates in a simple, powerful sequence:
1.   **Record:** Captures audio from the user's microphone via the browser.
2.   **Transcribe:** Converts the recorded audio into text using **OpenAI's Whisper**.
3.   **Generate:** Sends the transcribed text to **Cohere** to generate an intelligent, conversational response.
4.   **Synthesize & Play:** Converts the text response back into audio using **gTTS** and plays it automatically to the user.

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

##  Getting Started

Follow these steps to set up and run the project on your local machine.

### 1. Prerequisites

-   **Python 3.8 or newer**: Ensure it's installed and accessible from your terminal.
-   **FFmpeg**: This is a critical dependency. Download it from the [official website](https://ffmpeg.org/download.html ) and ensure its location is added to your system's `PATH` environment variable.

### 2. Installation

First, clone or download the repository to your local machine.

```bash
# Clone the repository
git clone https://your-repository-url.git

# Navigate into the project directory
cd your-project-directory
```

Next, install all the required Python packages using `pip`. It's highly recommended to do this within a virtual environment.

```bash
pip install Flask Flask-CORS openai-whisper cohere gTTS numpy scipy
```

### 3. API Key Configuration

This project requires an API key from Cohere to function.

1.  Navigate to the [Cohere website](https://cohere.com/ ) and create a free account to get your API key.
2.  Open the `app.py` file in a code editor.
3.  Locate the following line:
    ```python
    COHERE_API_KEY = "YOUR_REAL_API_KEY_HERE"
    ```
4.  Replace `"YOUR_REAL_API_KEY_HERE"` with the actual API key you obtained.

### 4. Running the Application

With all dependencies installed and keys configured, you can now run the server.

```bash
python app.py
```

Once the server is running, you will see output in your terminal indicating that it is active on `http://127.0.0.1:5000`.

### 5. Accessing the Chatbot

1.  Open your favorite web browser.
2.  Navigate to **`http://127.0.0.1:5000`**.
3.  The first time you use the microphone, your browser will ask for permission. **You must click "Allow"**.
4.  Click the microphone icon and start your conversation!

---

## Project Structure

The project directory is organized as follows to ensure Flask operates correctly.

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
