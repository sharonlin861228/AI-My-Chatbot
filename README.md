# My Chatbot - Ask About Me

Welcome to **My Chatbot**! This application allows you to ask questions about my professional experience, skills, and background. It uses AI-powered natural language processing to provide accurate and relevant answers based on my resume.

---

## **Objective**
The goal of this project is to create an interactive chatbot that can answer questions about my professional experience, skills, and background. The chatbot uses OpenAI's GPT model to process user queries and provide responses based on the content of my resume.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries and Frameworks**:
  - `streamlit`: For building the web interface.
  - `tiktoken`: For efficient token counting.
  - `PyPDF2`: For extracting text from PDF files (e.g., my resume).
  - `langchain`: For integrating language models and managing document-based question answering.
  - `faiss-cpu`: For efficient similarity search in vectorized documents.
  - `openai`: For accessing OpenAI's GPT models.
- **APIs**:
  - OpenAI API: To power the chatbot's natural language processing capabilities.

---

## **How to Use**

### **1. Prerequisites**
Before running the application, you need to:
1. **Apply for an OpenAI API Key**:
   - Sign up at [OpenAI](https://platform.openai.com/signup/).
   - Generate an API key from the OpenAI dashboard.
   - Replace the placeholder `OPEN_API_KEY` in the code with your actual API key.

2. **Install Required Libraries**:
   - Install the necessary Python libraries using `pip`:
  
  ```bash
   pip install streamlit tiktoken PyPDF2 langchain langchain-community faiss-cpu openai
```

3. **Replace the Resume:**:
    - Place your resume (in PDF format) in the project directory.

    - Update the path to the resume in the code:
```python
from PyPDF2 import PdfReader
pdf_reader = PdfReader('/path/to/your/resume.pdf')
```


### **2. Running the Application**

1. **Navigate to the project directory in your terminal.**

**Run the Streamlit application:**

```bash
streamlit run chatbot.py
```

2. **Open your browser and interact with the chatbot:**

- Type your questions in the input box.
- The chatbot will provide answers based on the content of the resume.

3. **Example Questions**

Here are some example questions you can ask:

- "What is your professional experience?"
- "What skills do you have?"
- "Tell me about your education background."
- "What projects have you worked on?"

## Project Structure

```
My-Chatbot/
├── chatbot.py            # Main application code
├── requirements.txt      # List of dependencies
├── README.md             # Project documentation
└── resume.pdf            # Your resume (PDF format)
```

## Installation Instructions

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
```

2. Navigate to the project directory:

```bash
cd your-repo-name
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the application:

```bash
streamlit run chatbot.py
```

## Customization

### Update Resume
Replace `resume.pdf` with your own resume.

### Add More Features
- Add more questions or functionalities to the chatbot.
- Customize the UI using Streamlit components.

### Deploy
Deploy the application using Streamlit Sharing, Heroku, or any other cloud platform.
