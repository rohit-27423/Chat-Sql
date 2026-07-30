# LangChain: Chat with SQL DB 🦜

A Streamlit web application that allows you to chat with your SQL databases using natural language. This project leverages **LangChain** and **Groq's Llama 3** models to translate user queries into SQL, execute them against the database, and return a human-readable response.

## Features

- **Natural Language to SQL**: Ask questions in plain English and get answers directly from your database.
- **Multiple Database Support**: 
  - Connect to a local SQLite database (`student.db`).
  - Connect to a remote MySQL database by providing host, user, password, and database name.
- **Powered by Groq & LangChain**: Uses Groq's high-speed inference API with the `llama-3.1-8b-instant` model and LangChain's zero-shot react SQL agent.
- **Interactive UI**: Built with Streamlit, providing an easy-to-use chat interface with message history.

## Prerequisites

- Python 3.8+
- A Groq API Key (get one at [console.groq.com](https://console.groq.com/))
- (Optional) MySQL database credentials if you want to use the MySQL feature.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/rohit-27423/Chat-with-SQL.git
   cd Chat-with-SQL
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open the app in your browser (usually `http://localhost:8501`).
3. In the sidebar:
   - Select your database type (SQLite or MySQL).
   - Enter your database credentials (if using MySQL).
   - Provide your **Groq API Key**.
4. Start chatting with your database!

## Files Description

- `app.py`: The main Streamlit application script containing the UI and LangChain agent logic.
- `sqlite.py`: A helper script to create and populate the initial SQLite database (`student.db`).
- `student.db`: A sample SQLite database included for quick testing.
- `requirements.txt`: List of Python packages required to run the project.

## License

This project is open-source and available under the [MIT License](LICENSE).
