🎬 YouTube Video Semantic Chunking
This project extracts audio from YouTube videos, transcribes it using OpenAI's Whisper model, and semantically chunks the transcriptions based on time segments. Ideal for speech analysis, summarization, or translation workflows.

🔍 Features
📥 YouTube Video Downloader: Automatically downloads video in the best quality.
🔊 Audio Extraction: Converts video to .mp3 audio using moviepy.
🧠 Speech-to-Text Transcription: Uses Whisper to transcribe audio with accurate timestamps.
✂️ Audio Segment Chunks: Splits audio and text into manageable chunks of configurable length (default: 15s).
🌐 Web UI with Gradio: Simple interface to enter a YouTube URL and get structured output.
📦 Installation
pip install yt-dlp pydub moviepy whisper gradio
Make sure you have ffmpeg installed and accessible in your system's PATH.

🚀 How to Use
Clone the repository or copy the script.

Run the script in your Python environment.

Use the Gradio interface to input a YouTube video URL.

Get JSON output with transcription, timestamp, and chunk information.

🧪 Sample Output
json
[
  {
    "chunk_id": 1,
    "chunk_length": 12.3,
    "text": "Welcome to the video on deep learning...",
    "start_time": 0.0,
    "end_time": 12.3
  },
  ...
]
📁 Project Structure
bash
📦youtube-chunker
 ┣ 📜main.py                # Main script
 ┣ 📜README.md              # Project documentation
🧠 Model Details
Model: Whisper (Base)

Source: OpenAI

Language: Supports multilingual transcription

🎓 Educational Use Case
This project was developed as a personal initiative to explore speech processing and video understanding through Whisper and Gradio. It’s useful for building tools for:

Lecture transcription

Podcast summarization

Video analytics

👨‍🏫 Supervision
Personal Project
Bachelor of Science, IIT Madras
Completed: October 2024
Faculty Advisor: Prof. Anand S

🙌 Acknowledgements
Whisper by OpenAI
yt-dlp
Gradio
Pydub
MoviePy
