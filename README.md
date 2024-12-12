## Prerequisites

Before running this application, ensure you have the following API keys:

- OpenAI API Key
- Groq API Key
- Pinecone API Key
- Pinecone Index Name

## Environment Setup

1. Clone the repository:
```bash
git clone https://your-repository-url.git
cd your-project-directory
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root and add your API keys:
```
OPENAI_API_KEY=your_openai_api_key_here
GROQ_API_KEY=your_groq_api_key_here
PINECONE_API_KEY=your_pinecone_api_key_here
PINECONE_INDEX=your_pinecone_index_name_here
```

## Running the Application

To start the Streamlit application:

```bash
streamlit run app.py
```

## Configuration

### API Keys
- **OpenAI API Key**: Used for [specific purpose, e.g., language model queries]
- **Groq API Key**: Used for [specific purpose, e.g., alternative language model or computation]
- **Pinecone API Key**: Used for vector database operations
- **Pinecone Index**: Specifies the specific Pinecone index to be used

## Security Notes

- Never commit your `.env` file to version control
- Add `.env` to your `.gitignore` file
- Rotate your API keys periodically
- Limit API key permissions to only what is necessary for the application

## Troubleshooting

1. Ensure all dependencies are installed correctly
2. Verify that your API keys are valid and have the necessary permissions
3. Check your internet connection
4. Confirm that the Pinecone index exists and is accessible

## Project Structure

```
project_root/
│
├── app.py             # Main Streamlit application
├── requirements.txt   # Python dependencies
├── .env               # Environment variables (not tracked in git)
├── .gitignore         # Git ignore file
└── README.md          # This documentation file
```
