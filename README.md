
# 📄 Info.ai – AI-Powered Document Chatbot  

Info.ai is an advanced **Retrieval-Augmented Generation (RAG)** chatbot designed for seamless interactions with documents. Built using **LangChain, LangGraph, and Google Vertex AI (Gemini-1.5)**, it ensures precise, document-aware responses, simplifying information retrieval.  

## ✨ Key Features  

✅ **AI-Driven Document Interaction** – Processes documents to provide contextually relevant answers.  
✅ **Efficient Retrieval & Generation Pipeline** – Built with **LangGraph** for modular execution.  
✅ **Smart Query Refinement** – Leverages **LangChain PromptTemplate** to clarify ambiguous queries.  
✅ **Multi-Tenant Capability** – Uses **Pinecone namespaces** and **MongoDB** to ensure isolated chat histories and vector searches.  
✅ **Scalable Document Processing** – Handles documents efficiently using **LangChain PyPDFLoader** and **RecursiveCharacterTextSplitter**.  
✅ **Real-Time AI Conversations** – Integrated with a dynamic **React.js frontend** for a smooth user experience.  

## 🛠 Tech Stack  

- **Backend**: LangChain | LangGraph | Flask | Pinecone | Google Vertex AI  
- **Database**: MongoDB | Pinecone Vector DB  
- **Frontend**: React.js  

## 🚀 Getting Started  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/your-username/Info.ai.git
cd Info.ai
```

### 2️⃣ Install Dependencies  
#### Backend  
```sh
cd backend
pip install -r requirements.txt
```

#### Frontend  
```sh
cd frontend
npm install
```

### 3️⃣ Set Up Environment Variables  
Create a `.env` file in both `backend/` and `frontend/` directories and configure the following:

#### Backend `.env`
```
MONGO_URI=<your-mongodb-uri>
PINECONE_API_KEY=<your-pinecone-api-key>
PINECONE_ENV=<your-pinecone-environment>
VERTEX_AI_PROJECT_ID=<your-gcp-project-id>
VERTEX_AI_MODEL=<your-gemini-model>
SECRET_KEY=<your-secret-key>
```

#### Frontend `.env`
```
REACT_APP_BACKEND_URL=http://localhost:5000
```

### 4️⃣ Run the Application  
#### Start Backend  
```sh
cd backend
python app.py
```

#### Start Frontend  
```sh
cd frontend
npm start
```

## 📌 API Endpoints  

### Upload Document  
```http
POST /upload
```
Uploads a document for processing.

### Chat with Document  
```http
POST /chat
```
Sends a query related to an uploaded document and receives AI-generated responses.

### Fetch Chat History  
```http
GET /history
```
Retrieves past chat history related to a specific document.

## 📜 License  
This project is licensed under the **MIT License**.

## 🤝 Contributing  
We welcome contributions! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Add new feature"`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a pull request.

## 📧 Contact  
For inquiries, reach out via email at `ridhamanand31@gmail.com` or open an issue on GitHub.
