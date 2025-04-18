
# 🤖 AI-Powered Code Reviewer

An intelligent code review platform built using **React** and powered by **Gemini (Google's AI)**. This application allows developers to upload or paste their code and receive real-time AI-driven suggestions, optimizations, and best practices to improve code quality.

---

## 📌 Overview

**AI Code Reviewer** is designed to mimic the feedback of an experienced developer. Whether you’re working solo or just want a second opinion on your code, this tool will:

- Analyze your code using Google's Gemini LLM
- Highlight potential bugs, code smells, and inefficiencies
- Suggest improvements, refactoring opportunities, and better practices
- Provide detailed reasoning behind each suggestion

---

## ✨ Features

- ✅ Paste or upload code in various languages
- ✅ Instant review powered by Gemini API
- ✅ Suggestions categorized by severity (e.g., warning, critical, style)
- ✅ Clean and interactive user interface
- ✅ Support for JavaScript, Python, Java, C++, and more
- ✅ Option to download review results

---

## 🔧 Tech Stack

| Tech           | Description                         |
|----------------|-------------------------------------|
| React          | Frontend framework                  |
| Tailwind CSS   | UI styling (optional but recommended)|
| Gemini API     | LLM for code review and generation  |
| Axios / Fetch  | API requests to Gemini              |
| Monaco Editor  | Code editor component (optional)    |
| dotenv         | Environment configuration           |

---

## 📂 Project Structure

```
ai-code-reviewer/
│
├── public/
├── src/
│   ├── components/       # Reusable UI components
│   ├── pages/            # Page-level views (e.g., Home, Review)
│   ├── services/         # Gemini API interactions
│   ├── utils/            # Helper functions for prompts, formatting
│   ├── App.jsx
│   ├── index.js
│   └── styles/
│
├── .env
├── package.json
└── README.md
```

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-code-reviewer.git
cd ai-code-reviewer
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Get Gemini API Key

- Visit [Google AI Studio](https://makersuite.google.com/app)
- Sign in with your Google Account
- Get your Gemini API Key

Create a `.env` file in the root:

```env
REACT_APP_GEMINI_API_KEY=your_api_key_here
```

> ⚠️ Keep this key secret in production. For full security, use a backend proxy for requests.

### 4. Run the App

```bash
npm start
```

Visit `http://localhost:3000` in your browser.

---

## 💬 Example Usage

### Example Prompt Sent to Gemini:

```json
{
  "prompt": "Please review the following JavaScript function for bugs and suggest improvements:\n\nfunction add(a, b) {\n return a + b;\n}"
}
```

### Example Response:

- ✅ Suggest adding type checks for `a` and `b`
- ⚠️ No validation if inputs are `undefined` or `null`
- 💡 Recommend using `Number()` conversion for safety

---

## 🖼️ Screenshots

> 📸 Add screenshots in this section to visually showcase your app.

```
Coming Soon...
```

---

## 📌 Roadmap

- [ ] GitHub integration for PR code reviews
- [ ] Inline suggestions with syntax highlighting
- [ ] Language auto-detection and tailored prompt logic
- [ ] User accounts and history of reviews
- [ ] Export review report as PDF or Markdown
- [ ] Dark mode toggle

---

## 🤝 Contributing

We welcome contributions! To contribute:

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙋 FAQ

### ❓ What languages are supported?
Currently, the app is optimized for JavaScript, Python, Java, C++, and C#. Support for other languages is experimental.

### ❓ Is the Gemini API free?
Google provides limited free usage, but extended use may require billing. Check [Gemini Pricing](https://ai.google.dev/pricing) for more details.

### ❓ Is this production ready?
This is a prototype/MVP. Security, performance, and backend validation should be added for production deployment.

---

## 🧠 Credits

- Built using [React](https://reactjs.org/)
- Powered by [Gemini](https://ai.google.dev/)
- Inspired by tools like GitHub Copilot, CodeWhisperer, and DeepCode

---

> Made with ❤️ for developers, by developers.
