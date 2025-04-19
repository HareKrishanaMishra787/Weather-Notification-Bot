# ☔ Weather Alert SMS Notifier

This Python project alerts you via SMS if rain is forecasted in your area within the next 12 hours. It uses the [OpenWeatherMap API](https://openweathermap.org/forecast5) for weather forecasting and [Twilio](https://www.twilio.com/) to send SMS messages.

## 📦 Features

- ⛅ Fetches 12-hour weather forecast data using OpenWeatherMap.
- 📱 Sends an SMS alert if rain is predicted (based on weather condition codes).
- ⚡ Uses Twilio API to deliver the message straight to your phone.

## 🚀 How It Works

1. Fetch weather forecast data for a specified location.
2. Analyze the weather condition codes.
3. If any code indicates rain (i.e., code < 700), send an SMS reminder to carry an umbrella.

## 🛠 Requirements

- Python 3.x
- [requests](https://pypi.org/project/requests/)
- [twilio](https://pypi.org/project/twilio/)

Install dependencies:

```bash
pip install requests twilio
```

## 🔐 Environment Variables

To keep your credentials safe, create a `.env` file or use environment variables for:

- `OPENWEATHER_API_KEY`
- `TWILIO_ACCOUNT_SID`
- `TWILIO_AUTH_TOKEN`
- `TWILIO_FROM_NUMBER`
- `TWILIO_TO_NUMBER`

> **Important:** Never hardcode API keys or secrets in your scripts. The current version includes sensitive information — be sure to remove or secure it before pushing to a public repository.

## 🧠 Code Overview

- `main.py`: Contains the main logic for fetching weather data and sending alerts.
- `.gitignore`: Ensures sensitive and unnecessary files like virtual environments aren't tracked.
- `pyvenv.cfg`: Part of the virtual environment setup.

## 🌍 Default Location

This project currently checks the weather for:

- **Latitude:** 25.317644  
- **Longitude:** 82.973915  
(Corresponding to Varanasi, India)

You can change this by modifying the `lat` and `lon` values in the script.

## 📤 Output

If rain is expected, you’ll receive a message like:

```
It's going to rain today. Remember to bring an ☔
```

## 📄 License

MIT License. Feel free to use, modify, and share this project.

---

**Happy Coding! Stay dry! ☔**
