# ✦ LUMI | AI-Powered Smart Task Planner

LUMI is a modern, aesthetic, and intelligent task planner built with **Streamlit** and Python. It leverages OpenRouter AI to parse natural language descriptions into structured, actionable tasks with automated priority detection, deadlines, and project organization.

---

## ✨ Features

- **🤖 AI Task Breakdown**: Enter free-form text or thoughts, and LUMI automatically extracts tasks, sets priorities (High, Medium, Low), and schedules dates.
- **📊 Interactive Dashboard**: Visual metrics for completion rate, overdue tasks, pending tasks, and interactive progress bars.
- **📋 Task Board**: Filter by project or priority, mark tasks complete, update due dates, and schedule reminders.
- **📁 Projects & Categories**: Organize your tasks into custom projects (General, Work, Personal, etc.).
- **💾 Local SQLite Persistence**: All tasks and state changes are stored persistently in a local SQLite database (planora.db).
- **🎨 Daylight Atelier Design System**: Styled following the [Impeccable](https://github.com/pbakaus/impeccable) design framework with high-contrast violet-slate typography, purposeful royal iris accents, tactile surfaces, and zero AI design slop.
- **📐 Impeccable AI Design Integration**: Built-in design system specifications (DESIGN.md, PRODUCT.md) and deterministic anti-pattern detection for AI coding agents.

---

## 🚀 Quick Start

### 1. Prerequisites
- Python 3.10+ (Python 3.12 recommended)
- Git

### 2. Clone the Repository
```bash
git clone https://github.com/rustedpotato/LUMI.git
cd LUMI
```

### 3. Create a Virtual Environment
```bash
# Windows
py -3.12 -m venv .venv
.\.venv\Scripts\activate

# macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Setup Secrets
Create a `.streamlit/secrets.toml` file in the project root:
```toml
OPENROUTER_API_KEY = "your-openrouter-api-key"
```

### 6. Run the Application
```bash
streamlit run app.py
```
Open [http://localhost:8501](http://localhost:8501) in your browser.

---

## 🎨 Impeccable Design System

LUMI integrates [pbakaus/impeccable](https://github.com/pbakaus/impeccable) to maintain design craft and prevent UI anti-patterns.

- **[PRODUCT.md](PRODUCT.md)**: Core product specifications, positioning, and operating context.
- **[DESIGN.md](DESIGN.md)**: Normative token schema (colors, typography, elevation, components, and named rules).
- **Scan for anti-patterns**:
  ```bash
  npx impeccable detect .
  ```

---

## 📂 Project Structure

```text
├── .agents/               # Impeccable agent skills & rules
├── .gemini/               # Gemini AI agent harness config
├── .cursor/               # Cursor agent integration
├── .claude/               # Claude Code harness config
├── .impeccable/           # Design sidecar and engine configuration
├── .streamlit/
│   ├── config.toml        # Streamlit configuration
│   └── secrets.toml       # API keys (ignored by git)
├── app.py                 # Core Streamlit application & logic
├── style.css              # Daylight Atelier design system stylesheet
├── DESIGN.md              # Impeccable design system specification
├── PRODUCT.md             # Product truth and operational context
├── planora.db             # SQLite database for task storage
├── requirements.txt       # Project dependencies
└── README.md              # Documentation
```

---

## 📄 License
This project is licensed under the MIT License.
