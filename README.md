# 🎬 Telegram Request Forwarder Bot

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Telegram](https://img.shields.io/badge/Telegram-Bot-green?logo=telegram)
![License](https://img.shields.io/badge/License-MIT-yellow)

A **Telegram bot** built with Python that manages movie and series requests by forwarding them to an admin group with structured formatting. Perfect for groups that handle requests efficiently.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| ✅ Request Validation | Accepts only messages starting with `#Request` |
| ✅ Auto Parsing | Extracts Name, Year, Quality, Language from requests |
| ✅ Admin Controls | Mark Done / Reject requests with inline buttons |
| ✅ ETA Handling | Customizable deadline for fulfilling requests |
| ✅ Easy Config | Configure BOT_TOKEN, ADMIN_CHAT_ID via `.env` |
| ✅ Error Handling | Handles forbidden access, timeouts, and invalid requests gracefully |

---

## 📝 Request Format

Users must send requests in the following format:

```text
#Request
Name: <Movie/Series Title>
Year: <Release Year>
Quality: <1080p/720p>
Language: <English/Hindi/Dual Audio>
Example:

text
Copy
Edit
#Request
Name: Example Movie
Year: 2024
Quality: 1080p
Language: Hindi
⚡ Tip: Include all fields for faster processing.

⚙️ Setup
Clone the repository

bash
Copy
Edit
git clone https://github.com/Ankit-Sharma1011/telegram-request-bot
cd direct-forward-bot
Create a virtual environment

bash
Copy
Edit
python -m venv venv
# Linux/macOS
source venv/bin/activate
# Windows
venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Create .env file
Copy .env.example and fill in your credentials:

env
Copy
Edit
BOT_TOKEN=your_bot_token_here
BOT_OWNER_ID=your_telegram_id
ADMIN_CHAT_ID=your_admin_group_chat_id
Run the bot

bash
Copy
Edit
python direct_forward_bot.py
🛠️ Commands
Command	Description
/start	Shows welcome message & ETA info
/help	Shows request format & usage instructions
/setdeadline <hours>	Owner only: change ETA for future requests

👥 Tips for Contributors / Usage
Fork the repo and create your own .env file with bot token and admin chat ID.

Never commit your .env; only commit .env.example.

Modify direct_forward_bot.py to add features like custom parsing, new buttons, or improved ETA logic.

Submit pull requests if you improve functionality (exclude secrets).

🖥️ Demo
You can add a screenshot or GIF showing the bot in action:


📂 Project Structure
lua
Copy
Edit
direct-forward-bot/
│-- direct_forward_bot.py
│-- requirements.txt
│-- README.md
│-- .gitignore
│-- .env.example


📜 License
MIT License – free and open-source.
