☁️ Rain Alert Notification System ☔
This project is a Rain Alert Notification System that sends an SMS notification when rain is forecasted. It integrates the OpenWeatherMap API for weather data and Twilio API for SMS notifications.<br>


<img src = "https://github.com/user-attachments/assets/2471ad31-a332-42c9-aea1-14c5828cf87f" height = "500">

📌 Features<br>
✅ Fetches weather forecast data for the next 12 hours<br>
✅ Identifies rainy conditions based on weather codes<br>
✅ Sends an SMS alert if rain is expected<br>
✅ Uses Twilio to send notifications<br>

🛠️ Tech Stack
Python

Requests (for API calls)

Twilio REST API (for sending SMS)

OpenWeatherMap API (for weather forecasting)

🚀 How It Works
Fetches weather data from OpenWeatherMap API for the specified location (Varanasi, India).

Checks if the weather condition ID is below 700 (indicating rain or snow).

If rain is detected, it triggers an SMS alert using Twilio.

The user receives a message:

"It's going to rain today. Remember to bring an ☔"

📦 Installation & Setup
🔹 Prerequisites
Python 3.x installed

Twilio account with a registered phone number

OpenWeatherMap API key

🔹 Steps
Clone this repository

sh
Copy
Edit
git clone https://github.com/your-username/Rain-Alert-Notification.git  
cd Rain-Alert-Notification
Install dependencies

sh
Copy
Edit
pip install requests twilio
Set up your API keys

Replace api_key, account_sid, and auth_token with your credentials in main.py.

Update to and from_ phone numbers with Twilio's verified numbers.

Run the script

sh
Copy
Edit
python main.py
🔒 Security Considerations
Do not expose your API keys in public repositories. Use environment variables or a .env file to store credentials.

📝 Future Enhancements
🔹 Add email notifications
🔹 Integrate push notifications for mobile apps
🔹 Extend to multiple cities

👨‍💻 Author
Hare Krishna Mishra

⭐ Contribute
If you find this project helpful, feel free to fork, improve, and submit a pull request!
