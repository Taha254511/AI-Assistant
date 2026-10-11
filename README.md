# 🤖 AI Assistant

An AI-powered personal assistant and email summarizer built with **Python, Flask, and Groq**. The application uses a large language model to answer user questions and summarize lengthy emails through a simple web interface.

## ✨ Features

### 💬 Personal AI Assistant

* Answers user questions using an AI language model.
* Provides helpful responses through an interactive web interface.
* Uses the Groq API with the `openai/gpt-oss-20b` model.

### 📧 Email Summarizer

* Summarizes lengthy emails into concise, easy-to-understand summaries.
* Generates summaries in approximately 2–3 sentences.
* Helps users quickly understand the main points of an email.

### 🌐 Web Interface

* Simple and user-friendly interface built with HTML and CSS.
* Flask handles backend requests and AI responses.
* Uses JSON responses to communicate with the frontend.

## 📸 Screenshot
<img width="1266" height="996" alt="Screenshot 2026-10-11 150600" src="https://github.com/user-attachments/assets/0bc31ca7-0c23-4a3d-9e5d-bc8a50073665" />
<img width="1247" height="536" alt="Screenshot 2026-10-11 150621" src="https://github.com/user-attachments/assets/3b19729c-785d-4572-bfc3-33ac9ec1e707" />


## 🛠️ Tech Stack

* **Language:** Python
* **Backend:** Flask
* **AI Model:** `openai/gpt-oss-20b`
* **LLM Provider:** Groq
* **API Client:** OpenAI Python SDK
* **Frontend:** HTML, CSS, JavaScript
* **Environment Variables:** python-dotenv

## 📁 Project Structure

```text
AI_Assistant/
│
├── static/
│   └── style.css
│
├── templates/
│   └── index.html
│
├── .gitignore
├── main.py
└── README.md
```

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/Taha254511/AI-Assistant.git
cd AI-Assistant
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows using Git Bash:

```bash
source .venv/Scripts/activate
```

### 3. Install Dependencies

Install the required Python packages:

```bash
pip install flask python-dotenv openai
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory and add your Groq API key:

```env
GROK_API_KEY=your_groq_api_key
```

Replace `your_groq_api_key` with your actual API key.

You can obtain an API key through the official [Groq Console](https://console.groq.com/).

### 5. Run the Application

Start the Flask development server:

```bash
python main.py
```

Open the local address displayed in your terminal, typically:

```text
http://127.0.0.1:5000/
```

You can now interact with the AI assistant and use the email summarization feature.

## 🔌 API Endpoints

| Endpoint     | Method | Description                                               |
| ------------ | ------ | --------------------------------------------------------- |
| `/`          | GET    | Renders the main web interface                            |
| `/ask`       | POST   | Processes user questions and returns AI-generated answers |
| `/summarize` | POST   | Summarizes email text and returns the summary             |

Both POST endpoints return JSON responses containing the generated text.

## 🔐 Security

* Store API keys in environment variables.
* Keep `.env` out of version control.
* Never expose API keys in source code or screenshots.
* Disable Flask debug mode when deploying the application publicly.

## 🎯 Future Improvements

* Add conversation history.
* Improve error handling for API failures.
* Support multiple AI models.
* Add copy-to-clipboard functionality for generated responses.
* Deploy the application for public access.

## 👨‍💻 Author

**Taha Hussain**<img width="1266" height="996" alt="Screenshot 2026-10-11 150600" src="https://github.com/user-attachments/assets/6afd7805-08a7-4d56-97e5-718538b06e3c" />

---

*Built with Python, Flask, and Groq to make everyday tasks easier with AI.*
