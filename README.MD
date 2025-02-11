# Bolashaq Q&A Chatbot

This is a multilingual AI chatbot built with **Rasa** to assist users with information about the Bolashak scholarship. The chatbot can answer frequently asked questions in **Kazakh, Russian, and English** and is designed to run on a local machine.

## Features
- **Multilingual Support** (Kazakh, Russian, English) using Google Translate API
- **Natural Language Processing (NLP)** powered by Rasa
- **Intent-based Responses** for accurate answers
- **Easy Deployment** on local machines or cloud platforms
- **Integration with Telegram, WhatsApp, and Web** (Optional)

## Installation
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/YOUR_USERNAME/bolashaq_chatbot.git
cd bolashaq_chatbot
```

### 2️⃣ Set Up a Virtual Environment
```sh
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

### 4️⃣ Train the Rasa Model
```sh
rasa train
```

### 5️⃣ Run the Chatbot
```sh
rasa shell
```

### 6️⃣ Run the Action Server
```sh
rasa run actions
```

## Configuration
### Edit `credentials.yml` to Connect with Telegram
```yaml
telegram:
  access_token: "YOUR_BOT_TOKEN"
  verify: "YOUR_BOT_USERNAME"
  webhook_url: "YOUR_WEBHOOK_URL"
```

### Running the Bot on a Web Interface
To enable API access, use:
```sh
rasa run -m models --enable-api --cors "*" --debug
```

## Contributing
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch and create a Pull Request.

## License
This project is open-source and available under the MIT License.

---
**Developed by:** ZhanEspo

