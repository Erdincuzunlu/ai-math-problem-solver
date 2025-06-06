# 🤖 Math AI Tutor (Mathpix + GPT-4 + Streamlit + Caching)

Math AI Tutor is an AI-powered educational app that allows students to **upload or photograph math problems**, extract the **equation using OCR**, and solve it **step-by-step using GPT-4** — just like a private tutor.

### 🧠 Key Features

- 🧾 **Upload or capture** a math question (PNG/JPG)
- 🔍 **Extracts LaTeX equation** using Mathpix OCR
- 💡 **Solves equation step-by-step** using GPT-4 Turbo
- 🧠 **Prompts GPT-4 with strict exam-style format** (LaTeX + numbered steps, no explanations)
- 💾 **Smart Caching with SQLite** — previously solved questions are fetched instantly to save cost
- 📐 **LaTeX-formatted output** — clean, exam-friendly display
- 💰 **Cost-efficient** — avoids duplicate GPT-4 calls, keeps API usage low
- ⚡ Built with **Streamlit** — fast prototyping and clean UI

---

### 🧱 Tech Stack

- Python 3.10+
- Streamlit
- Mathpix API
- OpenAI GPT-4 API
- SQLite (caching)
- Pillow
- Requests
- dotenv

---

### 🖥️ Demo (Coming Soon)

A demo video will be uploaded soon showing the full flow: image ➜ OCR ➜ GPT-4 ➜ solution.

---

### ⚙️ Installation

```bash
# Clone the repo
git clone https://github.com/Erdincuzunlu/math-ai-tutor.git
cd math-ai-tutor

# Install dependencies
pip install -r requirements.txt

# Rename the environment file
cp .env.example .env

# Then add your own API keys into .env:
# OPENAI_API_KEY=
# APP_ID=
# APP_KEY=

# Run the app
streamlit run app.py
