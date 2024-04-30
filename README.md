# UP Tourism Chatbot

This Python application is a chatbot designed specifically for promoting UP Tourism. It leverages various technologies and libraries to provide an interactive conversational experience.

## Requirements

Ensure you have the following libraries installed:

- `Langchain`
- `chromadb`
- `Streamlit`
- `Google-generativeai`
- `langchain-google-genai`
- `python-dotenv`
- `PyPDF2`

## Description

The UP Tourism chatbot is a versatile tool that offers multiple functionalities:

1. **PDF Processing:** Users can upload PDF files containing information about Uttar Pradesh tourism attractions. The chatbot processes these files using PyPDF2 to extract text for analysis.

2. **Text Analysis:** Extracted text is segmented into manageable chunks using `langchain`'s RecursiveCharacterTextSplitter for efficient processing.

3. **Vectorization:** The chatbot employs `google-generativeai` to generate embeddings for text chunks, which are then stored in a Faiss vector store using `langchain-vectorstores`.

4. **Question Answering:** With a conversational chain powered by `langchain.chains.question_answering`, the chatbot can answer user queries related to UP tourism. It uses pre-trained models and context from uploaded PDFs to provide accurate responses.

## Usage

1. Clone the repository or download the Python script.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Set up your Google API key in a `.env` file.
4. Run the application using `streamlit run chatbot.py`.
5. Upload PDF files, ask questions related to UP tourism, and interact with the chatbot to explore various tourist destinations.

## Configuration

Ensure you configure your `.env` file with the following content:
#### GOOGLE_API_KEY=your_google_api_key_here


Replace `your_google_api_key_here` with your actual Google API key.

## Additional Notes

- Customize the CSS styles in the code (`custom_css`) to modify the appearance of the Streamlit interface.
- Ensure your Google API key is properly configured and accessible for the chatbot to function seamlessly.
- Explore the `langchain` and `google-generativeai` documentation for advanced customization options and features.

## Acknowledgments

We acknowledge the contributions of various open-source libraries and frameworks that power this chatbot, including `langchain`, `google-generativeai`, `streamlit`, and others.

## Authors
-Manvi Sinha[@sinhamanvi17@gmail.com]

-Varnita S R[@varnitasr20@gmail.com]

## License

This project is licensed under the MIT License.

