# 🎥 VidSnapAI

Turn your memories into personalized video reels with ultra-realistic AI narration.

## ✨ What It Does

VidSnapAI is a full-stack web app that allows users to:
- 📸 Upload multiple images  
- 📝 Enter a custom description or story  
- 🗣️ Convert the text into **natural-sounding speech using ElevenLabs API**  
- 🎞️ Automatically generate a reel combining the photos and audio  
- 💾 Save the final video to a gallery within the website  

## 🛠 Tech Stack

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python (Flask)  
- **AI Voiceover:** ElevenLabs Text-to-Speech API  
- **Video Processing:** MoviePy  
- **Templating:** Jinja2  
- **Storage:** Local file system  

## 🔐 API Usage

This project uses [ElevenLabs API](https://www.elevenlabs.io/) to generate realistic voiceovers.
- Requires a free ElevenLabs account  
- API key is stored in `.env` for security  
- Handles fast and high-quality speech generation  

## 🚀 Live Demo

🔗 [Coming Soon / Add deployed link here]

## 📁 Repository Structure

<pre>
vidsnap-ai/
├── static/
│   ├── css/
│   ├── uploads/        # Uploaded images
│   ├── final/          # Generated reels
├── templates/
│   ├── index.html
│   ├── gallery.html
├── app.py              # Flask app
├── requirements.txt    # Python dependencies
</pre>

## 🧪 How to Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/namanj04/vidsnap-ai.git
cd vidsnap-ai
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```
### 3. Set up ElevenLabs API

1. Sign up at [ElevenLabs](https://www.elevenlabs.io/) and log in.  
2. Go to your **Profile → API Key** section and copy your API key.  
3. In the root directory of the project, create a `.env` file and add the following line:

### 4. In your Python code, make sure to load the API key like this:
```python
import os
api_key = os.getenv("ELEVENLABS_API_KEY")
```
### 5. Run the Flask app
```
python app.py
```
### 6. Open the app in Your browser
```
http://localhost:5000
```

## 🔄 Future Enhancements

- 🔐 Add user authentication (login/signup)
- ☁️ Store videos in cloud (AWS S3, Firebase, etc.)
- ⬇️ Enable download option for generated reels
- 🎙️ Add custom voice selection from ElevenLabs API
- 📱 Make UI fully responsive for mobile devices
- 🧼 Auto-clean old uploaded files to save disk space
- 📊 Add usage stats or dashboard for users
- 🎛️ Drag-and-drop support for image uploads


