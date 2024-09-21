# YouTube Video Transcriber

This repository contains a YouTube video transcriber that uses OpenAI's GPT-3.5 for answering questions based on the transcript of a YouTube video. The application extracts the transcript from the video, splits it into smaller chunks, and uses a vector database to allow for semantic search on the transcript. A simple Streamlit-based front end is provided for user interaction.

## Features

- Extracts the transcript from a YouTube video using `YoutubeLoader`.
- Splits the transcript into manageable chunks for efficient search and query.
- Allows users to ask questions about the video transcript.
- Uses OpenAI's GPT-3.5 to generate detailed and verbose responses based on the video transcript.
- Provides a simple and clean user interface with Streamlit.

## Technologies Used

- **LangChain**: For managing LLM chains, embeddings, and vector stores.
- **FAISS**: For building a vector database that enables similarity search.
- **Streamlit**: For creating a web-based frontend to interact with the transcriber.
- **OpenAI**: For generating responses using GPT-3.5.
- **YouTubeLoader**: To fetch the transcript from a YouTube video URL.

## Usage

1. Set up environment variables:
   - Create a `.env` file in the root directory of the project.
   - Add your OpenAI API key:
     ```
     OPENAI_API_KEY=your-openai-api-key
     ```

2. **Run the Streamlit App:**

   Start the Streamlit app by running the following command:
   ```bash
   streamlit run main.py
