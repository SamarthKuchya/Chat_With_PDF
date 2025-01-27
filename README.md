# Chat With PDF

Chat With PDF is a Streamlit-based application that enables users to interact with the content of PDF documents using natural language queries. By leveraging Google Generative AI embeddings and FAISS for vector-based searches, this project ensures accurate and detailed responses to user queries. The project was built for the BOB Hackathon, where it reached the finalist round.

## Features
- Upload multiple PDFs for processing.
- Extract text from PDFs and divide it into manageable chunks for efficient querying.
- Use FAISS for vector storage and similarity search.
- Generate accurate and detailed responses using Google Generative AI (Gemini model).
- Output formatted responses for structured information.

---

## Installation and Setup

### Prerequisites
1. Python 3.7 or higher.
2. Google API Key for Generative AI.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/SamarthKuchya/Chat_With_PDF.git
   cd chat_with_pdf
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project directory and add your Google API key:
   ```plaintext
   GOOGLE_API_KEY='your_api_key'
   ```

4. Run the application:
   ```bash
   streamlit run main.py
   ```

---

## Usage
1. Upload one or more readable PDF files through the sidebar menu.
2. Click on "Submit & Process" to process the PDFs.
3. Enter a question in the text input field to query the content of the uploaded PDFs.
4. View the response generated from the PDF content.

---

## How It Works
1. **Text Extraction**: Text is extracted from the uploaded PDFs using the `PyPDF2` library.
2. **Text Splitting**: The text is split into manageable chunks using the `RecursiveCharacterTextSplitter` from LangChain.
3. **Vector Store**: FAISS is used to create a vector store for efficient similarity searches.
4. **Conversational Chain**: Queries are handled using a QA chain built with Google Generative AI (Gemini model) and a custom prompt template.

---

## Project Highlights
- **Hackathon Achievement**: Finalist project at the BOB Hackathon.
- **Efficiency**: Handles large datasets with 10,000+ characters per chunk.
- **Accuracy**: Ensures responses are based strictly on the provided context, avoiding misinformation.

---

## Technologies Used
- **Frameworks and Libraries**: Streamlit, FAISS, PyPDF2, LangChain
- **AI Models**: Google Generative AI (Gemini)
- **Languages**: Python

---

## Contribution
Feel free to fork this repository and contribute to its development by submitting pull requests. Suggestions and feedback are always welcome!

---

## License
This project is licensed under the MIT License.

---

## Acknowledgments
Special thanks to the BOB Hackathon organizers and mentors for their guidance and support.

