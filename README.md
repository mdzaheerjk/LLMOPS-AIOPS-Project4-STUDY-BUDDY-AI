# 🤖 LLMOps & AIOps Project 4: Study Buddy AI

![LLMOps](https://img.shields.io/badge/LLMOPs-AIOps-blueviolet)
![Python](https://img.shields.io/badge/Python-3.12%2B-brightgreen)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Deploy-blue)
![Jenkins](https://img.shields.io/badge/Jenkins-CI%2FCD-success)
![License](https://img.shields.io/badge/License-GPL--3.0-orange)

A modern, production-grade AI-powered study assistant built with LLMOps and AIOps best practices. Study Buddy AI leverages Large Language Models, modular prompt engineering, and scalable infrastructure to generate personalized study questions, explanations, and learning resources. The system is designed for extensibility, observability, and robust cloud-native deployment.

> 📁 **Repository:** `LLMOPS-AIOPS-Project4-STUDY-BUDDY-AI`

---

## 🚀 Project Highlights

- 🎓 **AI Study Assistant:** Generate personalized study questions, quizzes, and learning content using LLMs.
- 🔗 **Prompt Engineering:** Modular, extensible prompt templates for flexible content generation.
- 🏗️ **Scalable Pipeline:** Modular codebase, config-driven, and ready for production.
- 🐳 **Dockerized:** Easy local or cloud deployment with Docker.
- ☸️ **Kubernetes-Ready:** Includes manifests for scalable deployment.
- 🔄 **CI/CD with Jenkins:** Automated build, test, and deploy pipeline.
- 📑 **Full Documentation:** See `FULL_DOCUMENTATION.md` for technical and usage details.

---

## 🧠 Technical Stack

- **Python 3.12+**
- **LLMs (Groq/OpenAI, via `src/llm/groq_client.py`)**
- **Prompt Engineering (custom templates)**
- **FastAPI/Flask (serving)**
- **Docker, Kubernetes, Jenkins**
- **Modern Python OOP & Pipeline Patterns**

---

## 🏗️ Project Structure

```bash
LLMOPS-AIOPS-Project4-STUDY-BUDDY-AI/
├── application.py                # FastAPI/Flask app entry point
├── src/
│   ├── __init__.py
│   ├── common/
│   │   ├── __init__.py
│   │   ├── custom_exception.py
│   │   └── logger.py
│   ├── config/
│   │   ├── __init__.py
│   │   └── settings.py
│   ├── generator/
│   │   ├── __init__.py
│   │   └── question_generator.py        # Core question/content generator
│   ├── llm/
│   │   ├── __init__.py
│   │   └── groq_client.py               # LLM API client logic
│   ├── models/
│   │   ├── __init__.py
│   │   └── question_schemas.py          # Pydantic models/schemas
│   ├── prompts/
│   │   ├── __init__.py
│   │   └── templates.py                 # Prompt template logic
│   └── utils/
│       └── __init__.py
├── manifests/
│   ├── deployment.yaml                  # Kubernetes deployment
│   └── service.yaml                     # Kubernetes service
├── Dockerfile
├── Jenkinsfile
├── requirements.txt
├── setup.py
├── LICENSE
├── README.md
├── FULL_DOCUMENTATION.md
```

---

## ⚡ Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/mdzaheerjk/LLMOPS-AIOPS-Project4-STUDY-BUDDY-AI.git
cd LLMOPS-AIOPS-Project4-STUDY-BUDDY-AI
```

### 2. Set up a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the application
```bash
python application.py
```
Or build and run with Docker:
```bash
docker build -t study-buddy-ai .
docker run -p 8000:8000 study-buddy-ai
```

### 5. Kubernetes Deployment
Apply the manifests to your cluster:
```bash
kubectl apply -f manifests/deployment.yaml
kubectl apply -f manifests/service.yaml
```

### 6. CI/CD with Jenkins
See `Jenkinsfile` for pipeline stages. Integrate with your Jenkins server for automated build/test/deploy.

---

## 🧪 Example Usage

- **Generate Study Questions:**  
  Input a topic or subject; get AI-generated questions or quizzes instantly.
- **Personalized Learning:**  
  Adaptive questions and explanations tailored to user level and topic.
- **API Demo or UI:**  
  Integrate as a backend for educational apps or chatbots.

---

## 📚 Documentation

See [FULL_DOCUMENTATION.md](FULL_DOCUMENTATION.md) for technical deep-dive, API reference, and extensibility guide.

---

## ✍️ Author

**Mohammed Zaheeruddin**  
🎓 First-Year B.Tech Student | AI/ML & GenAI Enthusiast  
🏫 Shetty Institute of Technology, Gulbarga  
📧 info.zaheerjk@gmail.com

---

## 📜 License

This project is licensed under the **GPL-3.0 License** – see the LICENSE file for details.

---

#### Key Features:
1. LLM-powered, modular AI study assistant
2. Clean, extensible Python codebase with prompt engineering
3. Docker, Kubernetes, and Jenkins for production-ready deployment
4. Designed for education, research, and real-world learning platforms
