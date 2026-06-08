# 🩺 Blood Work Analyzer

An AI-powered web app that analyzes blood work reports and provides
a personalized **health summary** and **Indian diet plan** using
Google Gemini and Streamlit.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-red?style=flat&logo=streamlit)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-AI-orange?style=flat&logo=google)
![LangChain](https://img.shields.io/badge/LangChain-green?style=flat)

---

## 📌 What Is This?

Most people get their blood work done but don't fully understand what
the results mean. This app solves that — paste your blood report and
instantly get a simple health summary and a practical Indian diet plan
tailored to your results.

---

## ✨ Features

- 📋 Paste your blood work report directly into the app
- 🤖 AI extracts and flags abnormal values (HIGH / LOW / NORMAL)
- 💊 Get a simple, easy-to-understand health summary
- 🥗 Receive a practical Indian diet plan based on your results
- 🌙 Clean dark themed UI built with Streamlit

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| [Streamlit](https://streamlit.io/) | Web UI |
| [Google Gemini](https://aistudio.google.com/) | AI model |
| [LangChain](https://www.langchain.com/) | LLM framework |
| [python-dotenv](https://pypi.org/project/python-dotenv/) | API key management |

---

## 🚀 How It Works

1. User pastes their blood work report
2. **Stage 1** — AI extracts all test values and flags HIGH / LOW / NORMAL
3. **Stage 2** — AI generates a health summary and Indian diet plan
4. Results are displayed in a clean scrollable UI

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/Sjkewat/blood-work-analyzer.git
cd blood-work-analyzer
```

### 2. Create a virtual environment
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Set up your API key
- Create a `.env` file in the root folder
- Copy the format from `.env_example`:
```
GEMINI_API_KEY=your_actual_api_key_here
```
- Get your free Gemini API key at: https://aistudio.google.com/

### 5. Run the app
```bash
streamlit run 2_Health_analys/streanlit_app/app.py
```
The app will open at `http://localhost:8501`

---

## 📁 Project Structure

```
blood-work-analyzer/
│
├── 1_simple_llm_calling/
│   └── Untitled.ipynb          # Simple LLM calling experiments
│
├── 2_Health_analys/
│   ├── blood_anayls.ipynb      # Blood analysis notebook
│   └── streanlit_app/
│       └── app.py              # Main Streamlit app
│
├── blood_work_analys.ipynb     # Main analysis notebook
├── main.py                     # Entry point
├── .env_example                # API key template
├── .gitignore                  # Ignores .env and sensitive files
├── pyproject.toml              # Project configuration
└── README.md                   # Project documentation
```

---

## 💻 Usage

1. Run the app using the command above
2. Paste your blood work report in the **left panel**
3. Click the **Analyze** button
4. View your results on the **right panel**:
   - 📊 Health Summary
   - 🥗 Indian Diet Plan

---

## 🔒 Privacy & Security

- Your `.env` file is **never uploaded** to GitHub
- Do **not** paste real patient data in a public setting
- The app runs **locally** on your machine
- No data is stored anywhere — all processing is done via Gemini API

---

## ⚠️ Disclaimer

This tool is for **educational purposes only** and is **not** a
substitute for professional medical advice.
Always consult a qualified doctor for medical decisions.

---

## 👨‍💻 Author

Made by **Suraj Kewat**
- GitHub: [@Sjkewat](https://github.com/Sjkewat)

---

## 📄 License

MIT License
