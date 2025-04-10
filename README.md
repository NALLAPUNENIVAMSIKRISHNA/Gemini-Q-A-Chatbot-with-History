#  Gemini Q&A Chatbot with Streamlit

Demo Video Link :- https://drive.google.com/file/d/1vyHZjJV3nMj16FYerUzecwd3wnP8KEOI/view?usp=sharing

This is a simple yet powerful **Q&A chatbot application** built using **Google’s Gemini Language Model (LLM)** and **Streamlit**. It allows users to ask questions and receive **real-time streamed responses** from the Gemini model. The app also maintains a **chat history** for a better conversational experience.

---

##  Key Features

-  **Google Gemini LLM Integration**: Uses the `gemini-2.0-pro-exp` model via Google Generative AI.
-  **Streamed Responses**: Gemini responses are streamed in real time for better user interaction.
-  **Session-based Chat History**: Chat history is preserved during the session to allow contextual conversations.
-  **Secure API Key Handling**: API keys are managed securely using `.env` and `python-dotenv`.

---

##  Project Structure

```
gemini-chatbot/
│
├── .env                # Contains your Gemini API key
├── app.py              # Main application logic using Streamlit
├── requirements.txt    # Python packages required
└── README.md           # Documentation for the project
```

---

##  Technology Stack

- **Frontend**: [Streamlit](https://streamlit.io/) – Python-based web framework for data apps.
- **Backend**: [Google Generative AI](https://ai.google.dev/) – Gemini LLM for text generation.
- **Configuration**: `python-dotenv` for managing environment variables securely.

---

##  Prerequisites

Before running the project, make sure you have the following:

- Python 3.8 or higher installed
- A valid [Google Generative AI API Key](https://makersuite.google.com/)
- Internet connection to access the Gemini API

---

## Installation & Setup

Follow these steps to get the app running locally:

### 1. Clone the Repository


### 2. Create a Virtual Environment (Optional but Recommended)

### 3. Install Required Dependencies

```bash
pip install -r requirements.txt
```

### 4. Add Your Google API Key

Create a `.env` file in the root directory and add the following line:

```
GOOGLE_API_KEY=your_google_api_key_here
```

Make sure your API key has access to the Gemini Pro model.

---

##  How to Run the App

Once the setup is complete, start the Streamlit app using:

```bash
streamlit run app.py
```

The app will open in your browser, typically at:  
**http://localhost:8501**

---

##  How It Works

1. The app loads the Gemini model and starts a fresh chat session.
2. A user enters a question using the input box.
3. The model sends a streamed response which is displayed in chunks.
4. The entire conversation (questions and answers) is saved in session state.
5. Users can view the chat history below the response area.

---

## 🧾 requirements.txt

Make sure this file contains the required dependencies:

```txt
streamlit
python-dotenv
google-generativeai
```

Install with:

```bash
pip install -r requirements.txt
```
