# ✦ LUMI | AI-Powered Smart Task Planner

LUMI is a modern, aesthetic, and intelligent task planner built with **Streamlit** and Python. It leverages OpenRouter AI to parse natural language descriptions into structured, actionable tasks with automated priority detection, deadlines, and project organization.

---

## ✨ Features

- **🤖 AI Task Breakdown**: Enter free-form text or thoughts, and LUMI automatically extracts tasks, sets priorities (High, Medium, Low), and schedules dates.
- **📊 Interactive Dashboard**: Visual metrics for completion rate, overdue tasks, pending tasks, and interactive progress bars.
- **📋 Task Board**: Filter by project or priority, mark tasks complete, update due dates, and schedule reminders.
- **📁 Projects & Categories**: Organize your tasks into custom projects (General, Work, Personal, etc.).
- **💾 Local SQLite Persistence**: All tasks and state changes are stored persistently in a local SQLite database (planora.db).
- **🎨 Custom Aesthetic UI**: Thoughtfully styled with soft lavender gradients, modern typography, and responsive cards.

---

## 🚀 Quick Start

### 1. Prerequisites
- Python 3.10+ (Python 3.12 recommended)
- Git

### 2. Clone the Repository
`ash
git clone https://github.com/rustedpotato/LUMI.git
cd LUMI
`

### 3. Create a Virtual Environment
`ash
# Windows
py -3.12 -m venv .venv
.\.venv\Scripts\activate

# macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
`

### 4. Install Dependencies
`ash
pip install -r requirements.txt
`

### 5. Setup Secrets
Create a .streamlit/secrets.toml file in the project root:
`	oml
OPENROUTER_API_KEY = "your-openrouter-api-key"
`

### 6. Run the Application
`ash
streamlit run app.py
`
Open [http://localhost:8501](http://localhost:8501) in your browser.

---

## 🌐 Deployment

### Deploying on Render
1. Create a new **Web Service** on [Render](https://render.com) and link your GitHub repo.
2. Configure settings:
   - **Runtime**: Python 3
   - **Build Command**: pip install -r requirements.txt
   - **Start Command**: streamlit run app.py --server.port  --server.address 0.0.0.0 --server.headless true
3. Add OPENROUTER_API_KEY under **Environment Variables**.

### Deploying on Streamlit Community Cloud
1. Visit [share.streamlit.io](https://share.streamlit.io) and select ustedpotato/LUMI.
2. Set the main file path to pp.py.
3. Add your OPENROUTER_API_KEY in **Advanced Settings -> Secrets**.
4. Click **Deploy**.

---

## 📂 Project Structure

`	ext
├── .streamlit/
│   ├── config.toml        # Streamlit configuration
│   └── secrets.toml       # API keys (ignored by git)
├── app.py                 # Core Streamlit application & logic
├── style.css              # Custom styling & themes
├── planora.db             # SQLite database for task storage
├── requirements.txt       # Project dependencies
└── README.md              # Documentation
`

---

## 📄 License
This project is licensed under the MIT License.
