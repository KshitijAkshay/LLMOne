# LLMOne 🤖

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=java)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5.9-green?style=for-the-badge&logo=spring-boot)
![Spring AI](https://img.shields.io/badge/Spring_AI-1.1.2-blue?style=for-the-badge&logo=spring)
![Docker](https://img.shields.io/badge/Docker-Enabled-blue?style=for-the-badge&logo=docker)

**LLMOne** is a powerful Spring Boot application that unifies access to multiple Large Language Models (LLMs) under a single, easy-to-use interface. It leverages **Spring AI** to connect with top-tier models from Google, OpenAI, Nvidia, and DeepSeek.

## ✨ Features

- **Unified API**: A single REST API to interact with multiple LLM providers.
- **Multi-Model Support**: Switch seamlessly between:
  - **MistralAI Devstral** (`mistralai/devstral-2512:free`)
  - **DeepSeek** (`tngtech/deepseek-r1t2-chimera:free`)
  - **Nvidia Nemotron** (`nvidia/nemotron-3-nano-30b-a3b:free`)
  - **GPT** (`openai/gpt-oss-120b`)
- **Modern Chat UI**: Includes a beautiful, responsive web interface built with React and Tailwind CSS.
  - Dark/Light mode support.
  - Real-time streaming-like experience.
  - Syntax highlighting for code.
- **Dockerized**: Ready for containerized deployment.

## 🖥️ Usage

### Web Interface

Open your browser and navigate to `http://localhost:8080` to use the chat interface.

### API Endpoints

You can also interact directly with the API:

| Model         | Method | Endpoint                   | Description               |
| :------------ | :----- | :------------------------- | :------------------------ |
| **MistralAI** | `GET`  | `/api/mistralai/{message}` | Chat with MistralAI       |
| **DeepSeek**  | `GET`  | `/api/deepseek/{message}`  | Chat with DeepSeek        |
| **Nvidia**    | `GET`  | `/api/nvidia/{message}`    | Chat with Nvidia Nemotron |
| **GPT**       | `GET`  | `/api/gpt/{message}`       | Chat with GPT             |

**Example:**

```bash
curl http://localhost:8080/api/mistralai/Hello
```

## 🛠️ Technologies Used

- **Spring Boot 3.5.9** - Backend Framework
- **Spring AI 1.1.2** - AI Integration
- **React & Tailwind CSS** - Frontend UI
- **Docker** - Containerization
- **Maven** - Dependency Management

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the project
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request
