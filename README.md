# LangChain Demo with Gemini API

This project demonstrates the implementation of a Language Learning Model (LLM) using **LangChain** and **Gemini** APIs. The app allows users to interact with a chatbot-like system that responds to their queries in a helpful manner.

---

## Features
- Integration with **LangChain** and **Google Gemini API**.
- Configurable parameters for model behavior such as temperature and maximum tokens.
- Uses environment variables for secure API key storage.
- Built using **Streamlit** for a simple and interactive UI.

---

## Prerequisites
1. Python 3.8 or above.
2. A Google Generative AI API Key.
3. Libraries mentioned in `requirements.txt` (LangChain, Streamlit, etc.).

---

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/langchain-demo-gemini.git
cd langchain-demo-gemini
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Configure API Keys
- Create a `.env` file in the project root directory:
  ```plaintext
  LANGCHAIN_API_KEY=wrong-api-key-here
  GOOGLE_API_KEY=wrong-api-key-here
  ```
  > **Note:** The `.env` file intentionally contains incorrect API keys. Replace them with your actual keys:
  ```plaintext
  LANGCHAIN_API_KEY=your-actual-langchain-api-key
  GOOGLE_API_KEY=your-actual-google-api-key
  ```

### 4. Run the Application
```bash
streamlit run app.py
```

---

## Usage
1. Enter a query/topic in the input field.
2. The app processes the query using the Gemini LLM and provides a response.
3. Replace the API keys in `.env` with valid ones if you encounter authentication errors.

---

## Notes
- The **LangChain** API key and the **Google API key** are required for this project to work.
- You can securely store your keys in the `.env` file.
- If you do not have a Google Generative AI API key, [click here](https://cloud.google.com/ai/) to get started.

---

## Troubleshooting
- **Incorrect API Key Error:** Ensure you’ve replaced the dummy API keys in the `.env` file with valid ones.
- **Dependency Issues:** Run `pip install -r requirements.txt` to ensure all dependencies are installed.
- **Environment Variable Not Set:** Use the `dotenv` library to load environment variables from the `.env` file.

---

## File Structure
```
langchain-demo-gemini/
├── app.py              # Main application code
├── .env                # Environment variables (ignored in Git)
├── requirements.txt    # Python dependencies
├── README.md           # Documentation
```

---
