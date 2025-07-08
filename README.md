# SummerizeMe

AI Video Summarizer
🎯 Overview
AI Video Summarizer is an intelligent application that automatically creates concise video summaries from longer videos. It combines computer vision, speech recognition, and natural language processing to generate meaningful video summaries while preserving the most important content.

✨ Features
🎥 Automated video summarization (30% of original length)
🔊 Audio transcription
📝 Text summary generation
👁️ Visual content analysis
📊 Interactive progress tracking
⬇️ Downloadable summaries and transcripts
🛠️ Technologies Used
Python: Core programming language
Streamlit: Web interface framework
YOLO: Object detection and visual analysis
Whisper: Audio transcription
OpenCV: Video processing
MoviePy: Video editing
DeepFace: Facial analysis (optional)
🚀 Installation
Clone the repository:
https://github.com/Mahith0534/SummarizeMe.git
cd ai-video-summarizer
Create and activate virtual environment:
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:
pip install -r requirements.txt
💻 Usage
Start the application:
streamlit run app.py
Open your web browser and navigate to http://localhost:8501

Upload a video file and wait for processing

Download or view the generated summaries

📁 Project Structure
ai-video-summarizer/
├── app.py                         # Main Streamlit application
├── modules/
│   ├── frame_extraction.py        # Frame extraction from video
│   ├── clip_selector.py          # Keyframe selection
│   ├── whisper_transcriber.py    # Audio transcription
│   ├── text_summarizer.py        # Text summarization
│   ├── visual_info_extractor.py  # Visual information extraction
│   ├── caption_overlay.py        # Caption overlay
│   ├── emotion_detector.py        # Emotion detection
│   └── video_summarizer.py       # Video summary generation
└── assets/
    ├── input_videos/            # Temporary storage for uploaded videos
    ├── keyframes/              # Extracted video frames
    ├── output/   
    ├── transcripts/
    │   └── summaries/   
    └── timestamps.txt    # Generated video summaries
⚙️ Configuration
The application can be configured through config.yaml:

Video summary length ratio
Minimum clip duration
Frame extraction interval
Model selection for analysis
📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
OpenAI Whisper for audio transcription
Ultralytics YOLOv8 for object detection
Streamlit for the web interface
DeepFace for facial analysis
