# Open Source Ai Chatbot

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:00B4DB,100:0083B0&height=220&section=header&text=Open%20Source%20Ai%20Chatbot&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Build%20Deploy%20And%20Own%20Your%20Conversational%20Ai&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-3.2.1-0083B0?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-88.9K-00B4DB?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-Apache_2.0-FF6B6B?style=for-the-badge&logo=apache&logoColor=white)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20api%20%7C%20docker-4A90E2?style=for-the-badge&logo=react&logoColor=white)

</div>

---

## 💬 Conversational AI Without Compromise

The AI chatbot market is dominated by closed-source giants that charge by the token, harvest your data, and dictate what your bot can and cannot say. **Open Source AI Chatbot** is the definitive alternative. It is a highly scalable, fully customizable, and completely open-source framework for building intelligent conversational agents that you truly own.

This repository provides everything you need to launch a production-ready AI chatbot in minutes. It features a modern, streaming-enabled chat interface, a robust backend for managing conversations, and seamless integration with a wide variety of LLM providers. Whether you want to build a customer support bot for your SaaS, a personal assistant for your Discord server, or a specialized domain expert, this framework handles the complex infrastructure.

Designed for developers who value privacy and control, the chatbot can be deployed entirely on your own infrastructure. You can run it with local models (via Ollama or vLLM) for maximum privacy, or connect it to external APIs (OpenAI, Anthropic) for maximum intelligence. The modular architecture means you can swap out components — like the vector database or the embedding model — without rewriting your entire application.

<img width="1668" height="943" alt="c2e515b0-db47-453a-aa7a-77a52e26d4fe" src="https://github.com/user-attachments/assets/8de9cf8c-56e0-4b52-b7b0-8e9b2f662a72" />


---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| ⚡ **Streaming Responses** | Real-time token streaming for a fluid, ChatGPT-like experience |
| 🧠 **Multi-Model Support** | Connect to OpenAI, Anthropic, Llama 3, Mistral, or any OpenAI-compatible API |
| 📚 **RAG Pipeline** | Built-in Retrieval-Augmented Generation to chat with your own documents |
| 🎨 **Customizable UI** | Fully responsive React frontend that can be deeply themed |
| 🗄️ **Persistent Memory** | Stores conversation history in PostgreSQL or SQLite for context retention |
| 🛡️ **Authentication** | Built-in JWT authentication and role-based access control |
| 🐳 **Docker Ready** | One-command deployment with Docker Compose |
| 🔌 **Plugin System** | Extend the bot with custom tools, web search, and API integrations |

---

## 🚀 Quick Setup

Get the chatbot running on your local machine. You will need Docker and Docker Compose.

```bash
# Clone the repository
git clone https://github.com/your-username/open-source-ai-chatbot.git

# Navigate into the directory
cd open-source-ai-chatbot

# Copy the environment template and add your API keys
cp .env.example .env

# Build and start the containers
docker-compose up -d --build
```

Once the containers are running, open your browser and navigate to `http://localhost:3000`. You will be greeted with the login screen. Create an admin account, and you can immediately start chatting. To use local models, ensure Ollama is running on your host machine, and select the local model option in the settings panel.

---

<div align="center">

### 🔗 Ready to launch your chatbot?

[![Get Chatbot](https://img.shields.io/badge/💬_GET_CHATBOT-00B4DB?style=for-the-badge&logoColor=white)](https://share.google/lHmUeWB471eVuSM6q)

</div>

---

## 🧠 The Architecture Of A Modern Chatbot

The chatbot is built on a microservices architecture, split into three main components: the **Frontend**, the **API Gateway**, and the **AI Worker**.

The **Frontend** is a React application built with Vite and Tailwind CSS. It manages the UI state, handles markdown rendering (with syntax highlighting for code blocks), and connects to the backend via WebSockets for real-time token streaming.

The **API Gateway** is a FastAPI server. It handles user authentication, conversation storage, and rate limiting. It acts as the central orchestrator, receiving user messages and routing them to the appropriate AI Worker.

The **AI Worker** is a separate, scalable service. It receives the prompt, constructs the final context window (including RAG documents if enabled), and sends the request to the LLM provider. By separating the AI Worker from the API Gateway, you can easily scale the number of workers to handle high traffic without slowing down the rest of the application.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-0083B0?style=for-the-badge&logoColor=white)](https://share.google/lHmUeWB471eVuSM6q)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that conversational AI should be open, transparent, and accessible to everyone. If you have ideas for new tools, improvements to the RAG pipeline, or want to help translate the UI, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-tool`).
3. **Commit** your changes (`git commit -m 'Add new tool'`).
4. **Push** to the branch (`git push origin feature/new-tool`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your bots, ask for help with prompt engineering, and discuss the latest trends in conversational AI.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@open-chatbot.dev.

---

<div align="center">

### ⭐ If this framework powers your project, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FF6B6B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/open-source-ai-chatbot)

---

### 🚀 Start building your chatbot today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-4A90E2?style=for-the-badge&logoColor=white)](https://share.google/lHmUeWB471eVuSM6q)

<sub>Crafted with precision and ❤️ by the Open Source AI Chatbot community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:0083B0,100:00B4DB&height=120&section=footer)

</div>
