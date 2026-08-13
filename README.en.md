# Microsoft-Style Chinese Translator

A fun translation tool based on the DeepSeek API that converts between Chinese, English, and "Microsoft-style Chinese" – letting you experience the unique, formal, slightly awkward, and humorous localization style used by Microsoft in its software.

## ✨ Features

- 🌐 Supports translation between **Chinese**, **English**, and **Microsoft-style Chinese**
- 🤖 Powered by the DeepSeek large language model for natural and stylistically appropriate translations
- 🔄 **Smart same‑language handling**: returns the original text directly when input and output languages match, saving API quota
- 📋 One‑click copy of translation results
- 🎲 Random examples for quick testing
- ⌨️ Keyboard shortcut `Ctrl+Enter` for fast translation
- 🎨 Glassmorphism UI with responsive design for mobile devices
- 📝 Fully open source, freely modifiable and deployable

## 🚀 Online Demo

You can visit the deployed version on GitHub Pages, Vercel, or other platforms.  
(*If no API key is configured, the page will prompt you to enter one.*)

## 📦 Local Setup

1. Clone the repository to your local machine.
2. Open `index.html` in your browser – no additional server required.

> **Note**: To use the translation feature, you need to configure your own DeepSeek API key (see below).

## 🔑 Configuring the API Key

1. Go to the [DeepSeek Platform](https://platform.deepseek.com/api_keys) to register and obtain your API key.
2. Open `index.html` and locate the JavaScript configuration section at the top of the file:
   ```javascript
   // ============================================================
   //  Configuration - Enter your DeepSeek API key here
   // ============================================================
   const API_KEY = 'YOUR_DEEPSEEK_API_KEY_HERE'; // Replace with your actual key
   const API_URL = 'https://api.deepseek.com/v1/chat/completions';
   const MODEL = 'deepseek-chat';
   // ============================================================
   ```
3. Replace `YOUR_DEEPSEEK_API_KEY_HERE` with your real API key.

> **Security Tip**: Do not commit code containing your API key to public repositories. Use environment variables or a backend proxy instead. This example is for demonstration only – in production, always keep your key secure.

## 🛠️ Tech Stack

- **Frontend**: Pure HTML5 + CSS3 + JavaScript (ES6)
- **UI Framework**: No dependencies, custom styles, Font Awesome icons
- **API**: DeepSeek Chat Completions API
- **Deployment**: Static files, can be hosted on any web server

## 📖 Usage Guide

1. **Select input language**: Choose the source language (Chinese, English, or Microsoft-style Chinese) from the "Input" dropdown.
2. **Select output language**: Choose the target language from the "Output" dropdown.
3. **Enter text**: Type or paste the content to be translated or polished into the text area.
4. **Translate**: Click the "Translate" button or press `Ctrl+Enter`.
   - If input and output languages are the same, the original text will be displayed directly (no API call).
   - Otherwise, the DeepSeek API will be called for translation.
5. **View result**: The translated text appears in the "Result" area below.
6. **Copy result**: Click the "Copy" button or click directly on the result box to copy the translation.
7. **Clear content**: Click the "Clear" button to reset the input and result areas.
8. **Random example**: Click "Random Example" to quickly fill in a sample sentence and automatically match the input language.

## 🤝 Contributing

Issues and Pull Requests are welcome! If you have suggestions or find bugs, feel free to participate.

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute it, provided you retain the original copyright notice.

---

**Enjoy the “Microsoft-style” translation! 😄**  
*This page may be performing an “error” operation, but your translation request has been successfully processed.*
