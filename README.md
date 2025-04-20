# 🛰️ ISS Overhead Notifier

A Python-based automation tool that alerts you via email when the International Space Station (ISS) is flying over your location **and** it's dark enough outside to see it. Never miss the chance to spot the ISS again! 🌌

---

## 📌 What It Does

This script:
- Tracks the real-time location of the ISS using public APIs.
- Checks whether it’s currently night at your location.
- Sends you an automated email if the ISS is overhead **and** the sky is dark—perfect viewing conditions!

---

## ⚙️ How It Works

It continuously:
1. Fetches the ISS's current latitude and longitude using the **Open Notify API**.
2. Uses the **Sunrise-Sunset API** to determine if it’s currently nighttime at your location.
3. If both conditions are true, it sends you an email saying the ISS is overhead and visible.

---

## 🛠 Technologies Used

- **Python** – Main programming language
- **Open Notify API** – For real-time ISS position
- **Sunrise-Sunset API** – For sunrise/sunset info
- `smtplib` – For sending email notifications
- `datetime` & `time` – For time-based checking
- `requests` – For making API calls

---

## 🚀 Setup Instructions

### 1. Clone the Repository

git clone https://github.com/your-username/iss-overhead-notifier.git
cd iss-overhead-notifier
---
### 2. Install Dependencies

pip install requests

### 3. Configure Your Details
Open the Python script and fill in these values:
MY_LAT = Your_current_latitude       # Example: 28.7041
MY_LONG = Your_current_longitude     # Example: 77.1025
MY_EMAIL = "your_email@gmail.com"    # Your Gmail address
MY_PASSWORD = "your_app_password"    # App password (NOT your Gmail login)

Note:

Use a Gmail App Password if you have 2-factor authentication enabled.
Never use your regular email password in the script.

### 4. Run the Script
python iss_notifier.py

🙌 Final Thought
With this tool running in the background, you’ll always know when to look up.
Catch the ISS as it orbits overhead—because some moments are too cosmic to miss. 🌍🚀
