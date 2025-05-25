# 🎥 Video Transcription and Summarizer

A Django-based web application that allows users to input YouTube video URLs and receive:
1. The full transcript of the video (if captions are available).
2. A concise, AI-generated summary of the content.

## 🚀 Features
- Fetch transcripts using the `youtube-transcript-api`.
- Summarize transcripts using Hugging Face's Transformer models (like T5 or BART).
- Display both full and summarized text in an intuitive interface.
- Error handling for invalid links or videos without subtitles.

## 🛠️ Tech Stack
- Backend: Django (Python)
- Frontend: HTML, CSS, Bootstrap
- NLP: Hugging Face Transformers (`transformers`, `torch`)
- APIs: `youtube-transcript-api`

## 📂 Project Structure
<pre>YT_summary/
├── transcript/ # Core app for transcription and summarization
│ ├── templates/ # HTML files
│ ├── static/ # CSS, JS
│ ├── views.py # View logic
│ ├── utils.py # API and ML utility functions
│ └── urls.py # URL routing
├── YT_summary/ # Project settings
├── db.sqlite3 # Database
└── manage.py # Django entry point</pre>


## ✅ How to Run
1. Clone the repository
2. Create a virtual environment and activate it
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Run migrations
   python manage.py migrate
5. Start the server
   python manage.py runserver
6. Access at http://127.0.0.1:8000

## Future Improvements
-Add support for multilingual videos.
-Include TTS (Text-to-Speech) for audio summaries.
-Store user transcript history with login feature.

## 🙌 Author
-Garvit Choudhary
-Divyansh Rana
