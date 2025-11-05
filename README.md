# RAG chatbot powered by 🔗 Langchain, OpenAI, Google Generative AI and Hugging Face 🤗

<div align="center">
  <img src="https://github.com/AlaGrine/RAG_chatabot_with_Langchain/blob/main/data/docs/RAG_architecture.png" >
  <figcaption>RAG architecture</figcaption>
</div>

## Project Overview <a name="overview"></a>

While Large Language Models (LLMs) are highly capable of generating intelligent and creative content, they rely on static training data, which can sometimes result in outdated or inaccurate responses. To address this limitation, **Retrieval Augmented Generation (RAG)** systems integrate LLMs with external data sources, enabling them to deliver more reliable and up-to-date answers.

This project focuses on developing a **RAG-based chatbot** using **LangChain**, powered by [OpenAI](https://platform.openai.com/overview), [Google Generative AI](https://ai.google.dev/?hl=en), and [Hugging Face](https://huggingface.co/) **APIs**. The chatbot allows users to upload documents in **txt**, **pdf**, **csv**, or **docx** formats and interact with their data conversationally. Relevant portions of the uploaded documents are retrieved and passed to the LLM, along with the user’s follow-up queries, to generate accurate and contextual responses.

Throughout the project, we explored every major component of the RAG pipeline — from the **document loader** to the **conversational retrieval chain**. We also built an intuitive front-end interface using [streamlit](https://streamlit.io/) for seamless user interaction.

---

## Installation <a name="installation"></a>

This project requires **Python 3** and the following key libraries:

`langchain`, `langchain-openai`, `langchain-google-genai`, `chromadb`, `streamlit`

The complete list of dependencies is available in the `requirements.txt` file.

---

## Instructions <a name="instructions"></a>

To run the application locally, follow these steps:

1. **Create a virtual environment:**  
   `python -m venv langchain_env`

2. **Activate the environment:**  
   On Windows:  
   `.\langchain_env\Scripts\activate`

3. **Navigate to the project directory:**  
   `cd RAG_Chatbot_Langchain`

4. **Install dependencies:**  
   `pip install -r requirements.txt`

5. **Launch the application:**  
   `streamlit run RAG_app.py`

6. **Configure settings in the sidebar:**  
   - Choose the LLM provider (**OpenAI**, **Google Generative AI**, or **Hugging Face**)  
   - Select a model (**GPT-3.5**, **GPT-4**, **Gemini-Pro**, or **Mistral-7B-Instruct-v0.2**)  
   - Adjust model parameters and add your API keys

7. **Create or load a Chroma vectorstore.**

8. **Start chatting with your documents!**  
   Ask questions and receive accurate, AI-generated answers.
