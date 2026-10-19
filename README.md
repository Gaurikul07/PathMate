# PathMate — Personal AI Assistant (Streaming Edition)

PathMate is an ultra-low-latency personal multimodal AI assistant that answers visual and general knowledge questions in real time using Google Gemini and computer vision.

---

## ✨ Features

- **⚡ Fast Streaming Architecture**:
  - Responses from Gemini stream token-by-token.
  - Buffered sentence-by-sentence streaming TTS (Text-to-Speech) begins speaking within ~1–2 seconds.
- **👁️ Multimodal Vision & Audio**:
  - Uses your webcam feed to give context-aware visual answers.
  - Continuous background microphone listening for wake word activation.
- **🗣️ Wake Word Activated**:
  - Simply say **"disha"** followed by your query or command.
- **🛡️ Secure Configuration**:
  - API keys and sensitive credentials managed via `.env` files.

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Gaurikul07/PathMate.git
cd PathMate
```

### 2. Set Up Virtual Environment
```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

> **Note for Windows users**: If PyAudio fails to install via pip, you can install pre-built wheels via `pip install pipwin && pipwin install pyaudio`.

### 4. Configure Environment Variables
Copy `.env.example` to `.env`:
```bash
cp .env.example .env
```
Open `.env` and paste your Google Gemini API key:
```env
GEMINI_API_KEY=your_actual_gemini_api_key_here
```

### 5. Run PathMate
```bash
python pathmate.py
```

---

## 🎮 Controls

- **Wake Word**: Say `"disha, [your question]"` to ask a question.
- **Quit**: Press `q` while focused on the webcam preview window to exit.

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).
