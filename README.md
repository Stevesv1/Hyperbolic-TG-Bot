# Hyperbolic AI Telegram Bot 🤖

A feature-rich Telegram bot integrating Hyperbolic.xyz's AI models for text generation, image creation, and audio synthesis.

## 📚 Features
- **Multi-Model Support**:
  - 📝 Text Generation (4 models)
  - 🖼️ Image Generation (2 models)
  - 🔊 Audio Synthesis (1 model)
- Secure API key management
- Interactive model selection
- Session-based interactions
- Easy switching between AI models

## 📋 Prerequisites
- Node.js v16+ 
- npm/yarn
- Telegram account & bot token
- [Hyperbolic.xyz](https://hyperbolic.xyz/) API key

## 📥 Installation
1. **Install Node.js and npm if not installed already**
```bash
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
```
2. **Clone Repository**
```bash
git clone https://github.com/Stevesv1/Hyperbolic-TG-Bot.git && cd Hyperbolic-TG-Bot
```
3. **Install dependencies**
```bash
npm install axios@^1.8.3 dotenv@^16.4.7 telegraf@^4.16.3 telegraf-session-local@^2.1.1
```

## ⚙️ Configuration
1. **Get Telegram Bot Token**
- Open Telegram and search for @BotFather
- Create new bot with /newbot
- Copy the provided HTTP API token

2. **Get Hyperbolic API Key**
- Sign Up or Log In at [Hyperbolic Website](https://hyperbolic.xyz)
- Go to Settings → API Keys
- Create/copy your API key

## 📁 Environment Set Up
- Create .env file using the below command
- nano .env and then input your Telegram Bot Token
```bash
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
```
- Now save this file using `Ctrl + X` and then `Y` and then press `Enter`

## ▶️ Run the bot
```bash
node bot.js
```

## 📜 Commands

| Command    | Description            |
|------------|------------------------|
| `/start`   | Start the bot          |
| `/switch`  | Change model           |
| `/remove`  | Remove API key         |
| `/help`    | Show commands          |

## 🔒 Security
- API keys stored only in session memory
- Keys automatically cleared with /remove command
- No persistent storage of credentials
