# 🎥 YouTube Video Analyzer Agent

An AI-powered YouTube Video Analyzer built with **Agno, Groq, GPT-OSS-20B, and Streamlit**. This project uses an AI agent to help users analyze YouTube video content and generate useful insights through a simple web interface.

## ✨ Features

* 🤖 AI agent powered by Agno.
* 🧠 Uses Groq's `openai/gpt-oss-20b` model.
* 🎥 Designed for YouTube video analysis.
* 🖥️ Interactive web interface built with Streamlit.
* 🔐 API credentials managed through environment variables.

## 🛠️ Tech Stack

* **Language:** Python
* **Agent Framework:** Agno
* **LLM Provider:** Groq
* **Model:** `openai/gpt-oss-20b`
* **Frontend:** Streamlit
* **Environment Management:** python-dotenv

## 📁 Project Structure

```text
youtube-video-analyzer/
│
├── ui.py
├── youtube_analyzer.py
├── requirements.txt
├── README.md
├── .gitignore
└── env                 # Local environment variables; not uploaded
```

## ⚙️ Prerequisites

Before running the application, install:

* Python 3.10 or a version compatible with your installed dependencies.
* Git.
* A Groq API key.

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/kulalsushma595-hue/youtube-video-analyzer.git
```

### 2. Navigate to the project directory

```bash
cd youtube-video-analyzer
```

### 3. Create a virtual environment

**Windows PowerShell:**

```powershell
python -m venv .venv
```

Activate it:

```powershell
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, you can run the commands below using the virtual environment's Python executable directly.

### 4. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 5. Configure your API key

Create a file named `env` in the project directory if your application expects that filename.

Add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Replace the placeholder with your actual API key.

**Security:** Never commit or upload your `env` file or expose your API key publicly.

If your application uses `load_dotenv()`, check whether it loads `env` explicitly. By default, `load_dotenv()` looks for `.env`, not a file named `env`.

### 6. Run the application

Start the Streamlit interface:

```bash
streamlit run ui.py
```

Streamlit should display a local address in your terminal. Open that address in your browser to use the application.


## 🔑 Environment Variables

The application uses the `GROQ_API_KEY` environment variable to access the Groq API.

Create a file named `env` in the project directory and add your API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Replace the placeholder with your actual Groq API key.

**Security:** Never upload your `env` file or expose your API key publicly.


Keep all credentials private. Never hardcode API keys in your Python files.

## 📌 Future Improvements

* Improve error handling and API failure messages.
* Add support for longer videos.
* Improve the presentation of summaries and insights.
* Add video transcript processing and analysis features where supported.

## 👩‍💻 Author

**Sushma Kulal**

GitHub: [kulalsushma595-hue](https://github.com/kulalsushma595-hue)

---

If you find this project useful, consider giving the repository a ⭐ on GitHub!
