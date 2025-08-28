````markdown
# Retrieval-Augmented Generation (RAG) System

This project is my implementation of a **Retrieval-Augmented Generation (RAG) system** built with **Java Spring Boot**.  
It allows users to upload PDFs, store embeddings in **PostgreSQL with pgvector**, perform semantic search, and generate context-aware answers using **OpenAI GPT**.  


## 🚀 Features
- Upload PDFs and automatically extract text.
- Generate and store embeddings with **pgvector**.
- Perform semantic search to retrieve the most relevant content.
- REST APIs for natural language Q&A.
- **React frontend** for document upload and interactive Q&A.
- Fully containerized with **Docker**.

---

## 🛠️ Tech Stack
- **Backend**: Java 21, Spring Boot, Spring AI  
- **Database**: PostgreSQL + pgvector  
- **Frontend**: React  
- **LLM Integration**: OpenAI GPT  
- **Deployment**: Docker, Docker Compose  


## ⚡ Getting Started

### Prerequisites
- Java 21+
- Maven or Gradle
- Docker & Docker Compose
- PostgreSQL with pgvector
- OpenAI API key

### Setup Instructions
````
1. Clone the repository:
   ```bash
   git clone https://github.com/PIYUSHBONDE/RAG-System.git
   cd RAG-System

2. Start PostgreSQL with pgvector:

   ```bash
   docker-compose up -d
   ```

3. Configure environment variables in a `.env` file inside `backend/`:

   ```env
   SPRING_DATASOURCE_URL=jdbc:postgresql://localhost:5432/rag_system
   SPRING_DATASOURCE_USERNAME=postgres
   SPRING_DATASOURCE_PASSWORD=postgres
   OPENAI_API_KEY=your_openai_api_key
   ```

4. Run the backend:

   ```bash
   cd backend
   mvn spring-boot:run
   ```

5. Run the frontend:

   ```bash
   cd frontend
   npm install
   npm start
   ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser.


## 📖 Usage

* Upload a PDF through the UI.
* Ask a question in natural language.
* The system retrieves relevant chunks and uses GPT to return an accurate, context-aware answer.


## 🔮 Future Improvements

* Multi-user support with authentication.
* Support for additional document types (Word, TXT).
* Improved ranking algorithms for semantic search.
* Integration with more LLM providers.


## 📎 Repository

This project is maintained under my account:
👉 [RAG System on GitHub](https://github.com/PIYUSHBONDE/RAG-System)

