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
