# PDF Chatbot using Flask and LangChain

## Overview
This project is a chatbot application that allows users to upload a PDF file and ask questions about its content. It utilizes **Flask** for the backend, **LangChain** for processing and understanding the document, and **HTML, CSS and JavaScript** for the frontend.

## Features
- Upload and process PDF documents
- Ask questions based on the PDF content
- Get AI-powered responses using LangChain
- REST API for frontend-backend communication
- Interactive user interface built with Vue.js

## Technologies Used
- **Flask** - Backend API and server
- **LangChain** - PDF processing and question answering
- **HTML, CSS and JavaScript** - Frontend for chatbot interface
- **PyMuPDF** - Extracting text from PDFs
- **OpenAI API** - Powering chatbot responses

## Installation

### Prerequisites
Make sure you have the following installed:
- Python 3.8+
- Node.js & npm (for frontend)

### Backend Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/SanjayKMangrani/PdfChatbot.git
   cd pdf-chatbot/backend
   ```
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask server:
   ```bash
   flask run
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the Vue.js app:
   ```bash
   npm run dev
   ```

## Usage
- Open the frontend in your browser.
- Upload a PDF file.
- Type a question related to the PDF content.
- Receive AI-generated responses based on the document.

## API Endpoints
### Upload PDF
- **POST** `/upload`
- **Description**: Uploads a PDF for processing.
- **Request**: `multipart/form-data` with a file.
- **Response**: `{'message': 'File uploaded successfully'}`

### Ask a Question
- **POST** `/chat`
- **Description**: Sends a user query and gets a response.
- **Request**: `{'question': 'Your question here'}`
- **Response**: `{'answer': 'AI-generated response'}`

