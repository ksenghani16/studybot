# StudyBot

StudyBot is an AI-powered chatbot designed to assist with studying and learning. It uses advanced language models to provide educational explanations, remembers user details across conversations, and maintains chat history for personalized interactions.

## Features

- Interactive chatbot for educational queries
- Personalized responses based on conversation history
- Simple API endpoints for integration
- CORS support for web applications

## Technologies Used

- **FastAPI**: Web framework for building APIs
- **LangChain**: Framework for building LLM applications
- **Groq API**: Language model provider
- **MongoDB**: Database for storing chat history
- **Python**: Programming language

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/ksenghani16/studybot.git
   cd studybot
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   Create a `.env` file with:
   ```
   GROQ_API_KEY=your_groq_api_key
   MONGODB_URI=your_mongodb_connection_string
   ```

## Usage

Run the application:
```
uvicorn app:app --reload
```

The API will be available at `http://localhost:8000`.

### API Endpoints

- `GET /`: Welcome message
- `POST /chat`: Send a chat message
  - Request body: `{"user_id": "string", "question": "string"}`
  - Response: `{"response": "string"}`

## Contributing

Feel free to submit issues and pull requests.

## License

This project is licensed under the MIT License.