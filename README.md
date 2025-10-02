# 🚀 GenAI Flask App: Evaluating and Comparing LLMs

This repository contains the project developed during the Coursera guided lab **"Hands-on with GenAI: Choosing the Right Model for Your Application"**.  
The primary goal is to build a web application using Flask that integrates with multiple Large Language Models (LLMs).  
The project focuses on obtaining structured outputs and comparing the performance of different models like **Llama 3, Granite, and Mixtral**.

---

## 🌟 Key Features

- **Flask Web Application**: Provides a simple interface for interacting with the AI models.  
- **LLM Integration**: Leverages the `ibm-watsonx-ai` library for seamless access to advanced Language Models.  
- **Structured Output (JSON)**: Implements LangChain's `JsonOutputParser` to ensure that the AI responses are consistently structured and easily consumed by the application.  
- **Prompt Engineering**: Utilizes specific prompt templates designed to generate actionable JSON responses.  
- **Model Evaluation**: Facilitates a practical comparison of leading LLMs (Llama 3, Granite, and Mixtral) based on criteria like latency and quality.  
- **Modular Code**: AI logic is encapsulated in reusable components, making the application easy to maintain and scale.  

---

## 🛠️ Technologies Used

| Component      | Technology     | Purpose                                           |
|----------------|---------------|---------------------------------------------------|
| Framework      | Python, Flask | Backend and routing for the web application.      |
| LLMs Platform  | IBM watsonx.ai| Provides access and deployment for the LLMs.      |
| Orchestration  | LangChain     | Manages prompt sequences and output parsing.      |
| Models         | Llama 3, Granite, Mixtral | Models used for comparative analysis. |

---

## ⚙️ Setup and Execution

Follow these steps to set up and run the application locally.

### 1. Clone the Repository
```bash
git clone https://github.com/carlosbkm/genai_flask_app_coursera.git
cd genai_flask_app_coursera
```

### 2. Create and Activate the Virtual Environment
Always use a virtual environment to manage dependencies:

```bash
# Create the environment
python -m venv venv

# Activate the environment (macOS/Linux)
source venv/bin/activate

# Activate the environment (Windows)
venv\Scripts\activate
```

### 3. Install Dependencies
Install all required Python packages from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 4. Configure Credentials
The project requires authentication to the watsonx.ai platform.

- Obtain your **API Key** and the **Project ID** from your watsonx.ai account.  
- Create a file named `.env` in the root of the project directory.  
- Add your credentials to the file as shown below:

```bash
# .env
WATSONX_API_KEY="YOUR_API_KEY_HERE"
WATSONX_PROJECT_ID="YOUR_PROJECT_ID_HERE"
```

### 5. Run the Application
Start the Flask development server:

```bash
python app.py  # Or the name of your main Flask file
```

The application will now be running and accessible in your browser at **http://127.0.0.1:5000**.

---

## 📝 Learning Summary

This project demonstrates proficiency in modern GenAI development workflows, specifically focusing on:

- **API Authentication**: Securely connecting a local application to a cloud-based LLM service.  
- **Controlled Output**: Mastering the use of `JsonOutputParser` to reliably integrate LLM output into backend code.  
- **Model Selection**: Applying practical criteria (latency, response quality) to make informed decisions about which LLM is best suited for a given application.  

---

## 🧑‍💻 Contributing

This repository was created as a guided project. However, feel free to fork it, modify it, and experiment with different models or prompt strategies!

---

Created by Carlos Garcia.
