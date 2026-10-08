# SnapBite

SnapBite is a simple nutrition helper that lets you:
- upload a photo of food
- ask what it is
- get a rough calorie and macro estimate
- send a summary to WhatsApp

It uses AI to look at the meal and explain it in plain language.

## What it does

- Takes a photo or text description of a meal
- Estimates calories, protein, carbs, and fat
- Shows the response in the app
- Sends a summary message to WhatsApp

## Tech used

- Python
- Streamlit
- Google Gemini AI
- Twilio WhatsApp API

## Setup

1. Clone the repo
2. Open the project folder
3. Create a virtual environment
4. Install dependencies

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Run locally

```bash
streamlit run app.py
```

## Required secrets

Create a `.streamlit/secrets.toml` file with your keys like this:

```toml
GEMINI_API_KEY = "your-google-api-key"
TWILIO_ACCOUNT_SID = "your-twilio-account-sid"
TWILIO_AUTH_TOKEN = "your-twilio-auth-token"
TWILIO_WHATSAPP_FROM = "whatsapp:+14155238886"
TWILIO_CONTENT_SID = "your-twilio-content-sid"
```

## Notes

This app is meant to give rough estimates, not exact nutrition tracking. It is designed to be simple and useful for everyday meal checking.

## License

This project is for personal or demo use.
