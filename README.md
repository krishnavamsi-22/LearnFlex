# LearnFlex – AI-Powered Learning Assistant

LearnFlex is an AI-powered learning assistant designed to make learning more interactive, personalized, and accessible. It leverages Large Language Models (LLMs), LangChain, and Retrieval-Augmented Generation (RAG) to generate structured learning content and support knowledge-based learning.

The application helps learners understand complex topics, explore concepts at different levels, and engage with AI-assisted learning experiences.

## ✨ Features

- **AI-Powered Content Generation:** Generate structured learning material using Large Language Models.
- **Multi-Level Learning:** Organize learning content into different levels of complexity.
- **Intelligent Question Answering:** Retrieve relevant information and generate context-aware responses.
- **Dynamic Quiz Generation:** Create quizzes to evaluate understanding and reinforce learning.
- **Document-Based Learning:** Leverage knowledge retrieval to work with learning resources.
- **Interactive Interface:** User-friendly Streamlit interface for an engaging learning experience.
- **Conversation Management:** Maintain learning conversations through session-based storage.

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Frontend | Streamlit |
| LLM Framework | LangChain |
| AI Model | Llama 3.1 70B Versatile |
| LLM Provider | Groq |
| Vector Database | ChromaDB |
| Machine Learning | PyTorch, Transformers |
| Audio Processing | Librosa |
| Configuration | YAML |
| Environment Management | Python Dotenv |

## 📂 Project Structure

```text
LearnFlex/
│
├── app/                    # Application interface and workflows
├── chat_sessions/          # Conversation session storage
├── models/                 # AI and model-related components
├── utils/                  # Utility functions and helpers
│
├── .devcontainer/          # Development environment configuration
├── config.yaml             # Model and application configuration
├── requirements.txt        # Python dependencies
├── pdf_download.py         # PDF download utility
├── usefull.py              # Supporting utility module
│
├── AI_ML_NLP_Definitions.pdf
├── Intro_to_AI_NLP_ML.pdf
├── LICENSE
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/krishnavamsi-22/LearnFlex.git

cd LearnFlex
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows:**
```bash
venv\Scripts\activate
```

**macOS / Linux:**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory and add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key
```

Obtain an API key from [Groq Console](https://console.groq.com/).

### 5. Run the Application

Run the Streamlit application using its main entry-point file:

```bash
streamlit run app/<entry_file>.py
```

Replace `<entry_file>.py` with the actual Streamlit application filename inside the `app` directory.

## 🔧 Configuration

LearnFlex uses `config.yaml` to manage model and application settings.

Example configuration:

```yaml
model_path:
  llama: "llama-3.1-70b-versatile"

temperature: 0

sessions_dir: "./chat_sessions/"

database: "./database/"
```

You can modify the configuration to adjust the model and application storage settings.

## 🧠 How It Works

1. **User Interaction:** Learners interact with the application through the Streamlit interface.
2. **Input Processing:** User queries and learning requests are processed by the application.
3. **LLM Integration:** LangChain connects the application with the Groq-hosted Llama model.
4. **Knowledge Retrieval:** Relevant information can be retrieved using the vector database.
5. **Response Generation:** The language model generates contextual learning content and responses.
6. **Session Management:** Conversation data is maintained using session-based storage.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `GROQ_API_KEY` | API key required to access Groq-hosted language models |

**Note:** Never commit your `.env` file or expose API credentials in the repository.

## 🚀 Future Enhancements

- Personalized learning paths based on learner progress.
- Advanced quiz analytics and performance insights.
- Expanded document-based knowledge retrieval.
- Improved conversational learning experiences.
- Additional AI-powered learning and assessment features.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Krishna Vamsi**

- GitHub: [@krishnavamsi-22](https://github.com/krishnavamsi-22)

---

*LearnFlex – Making learning smarter, more interactive, and AI-powered.*
