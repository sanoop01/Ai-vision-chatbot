# 🥗 MacroSnap — AI Vision Nutrition Buddy

MacroSnap is a **Streamlit-based AI nutrition assistant** that uses **Gemini AI** to analyze food images and answer nutrition-related questions.

Users can upload a meal photo to get estimated **calories, protein, carbohydrates, and fat**. The app can also send the user's daily meal summary to **WhatsApp using Twilio**.

## 📁 Project Structure

```text
MacroSnap/
├── app.py
├── prompts.py
├── requirements.txt
├── .gitignore
├── README.md
└── .streamlit/
    ├── secrets.toml.example
    └── secrets.toml
```

## 🚀 Installation

Activate the virtual environment:

### Windows PowerShell
```powershell
.\venv\Scripts\Activate.ps1
```

### Windows CMD
```cmd
venv\Scripts\activate.bat
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## 🔑 API Configuration

Create:

```text
.streamlit/secrets.toml
```

Add your:

```toml
GEMINI_API_KEY = "your-api-key"
TWILIO_ACCOUNT_SID = "your-account-sid"
TWILIO_AUTH_TOKEN = "your-auth-token"
TWILIO_WHATSAPP_NUMBER = "whatsapp:+14155238886"
TWILIO_CONTENT_SID = "your-content-sid"
```

Get the Gemini API key from [Google AI Studio](https://aistudio.google.com/?utm_source=chatgpt.com) and Twilio credentials from [Twilio Console](https://console.twilio.com/?utm_source=chatgpt.com).

## ▶️ Run the Application

```bash
streamlit run app.py
```

Open:

```text
http://localhost:8501
```

## ☁️ Deployment

The application can be deployed using **Streamlit Community Cloud**.

1. Push the project to GitHub.
2. Do not upload `secrets.toml`.
3. Create a new app on Streamlit Cloud.
4. Select `app.py`.
5. Add your secrets in **Settings → Secrets**.
6. Deploy.

## 🛠️ Technologies

- Python
- Streamlit
- Gemini AI
- Twilio WhatsApp API

> **Note:** Nutrition values provided by the AI are estimates and should not replace professional dietary advice.