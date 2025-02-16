# Movie Recommendation Chatbot

This project is a Flask-based web application that provides movie recommendations based on user queries. It uses advanced language models and vector-based search to retrieve and rank movie suggestions. The system integrates multiple AI-powered APIs and models to ensure an engaging and accurate chatbot experience.

---

# Live

You can play with the testbot with the link below.
Note that it requires 1 minute to startup after trigger because it goes idle when it is not used.
https://cinechatrag.onrender.com/

## Features

- **Movie Recommendations:** Suggests movies based on user input and retrieves relevant titles with detailed metadata.
- **Flask-based Web Interface:** Simple and user-friendly web interface for interaction.
- **AI-Powered Search:** Uses OpenAI embeddings and self-query retrievers to find the most relevant movies.
- **Customizable Backend:** Supports Groq and OpenAI models for dynamic query handling.

---

## Prerequisites

1. **Python 3.12.8 or later**: Ensure you have Python installed.
2. **API Keys**: Set up API keys for OpenAI and Groq.
3. **Environment**: `pip` and `virtualenv` or any Python environment manager.

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/movie-recommendation-chatbot.git
   cd movie-recommendation-chatbot
   ```

2. **Create and Activate a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**:
   - Create a `.env` file in the project directory.
   - Add the following variables:
     ```env
     OPENAI_API_KEY=your_openai_api_key
     GROQ_API_KEY=your_groq_api_key
     PORT=5000  # Optional, default is 5000
     ```

5. **Prepare the Dataset**:
   - Place the `CineChatCSV_cleaned_new.csv` file in the root directory.

---

## Running the Application

1. **Start the Application**:
   ```bash
   python app.py
   ```

2. **Access the Application**:
   - Open a web browser and navigate to `http://localhost:5000`.

---

## Usage

- Use the chatbot interface to ask for movie recommendations or details.
- The chatbot will return:
  - A list of movie suggestions with metadata (title, year, rating, etc.).
  - A response based on your query generated by the AI model.

---

## Project Structure

```
movie-recommendation-chatbot/
|
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── templates/
│   └── chat.html           # HTML template for the chatbot UI
├── static/
│   └── styles.css          # CSS for UI styling (if any)
├── CineChatCSV_cleaned_new.csv  # Input dataset
├── .env                    # Environment variables file
└── README.md               # Documentation
```

---

## Notes

- Ensure the `movie_vectorstore5openai` directory exists or will be created during runtime for vector storage.
- Use the latest versions of dependencies to avoid compatibility issues.

---

## Troubleshooting

- **Missing API Keys**: Verify the `.env` file contains valid API keys.
- **Dependency Issues**: Run `pip install --upgrade -r requirements.txt` to update dependencies.
- **Port Conflicts**: Modify the `PORT` variable in the `.env` file to use a different port.

---

## Demo Video

[Watch the project demo on YouTube](https://www.youtube.com/watch?feature=shared&v=Q5oloQnzzVM)
