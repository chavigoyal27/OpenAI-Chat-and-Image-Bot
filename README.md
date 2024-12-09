---
title: "Personal Chatbot and Image Generator"
output: github_document
---

# Personal Chatbot and Image Generator

This project is a web application built using FastAPI that allows users to interact with a personal chatbot powered by OpenAI's GPT-4 and generate images based on text prompts using OpenAI's DALL·E.

## Features

- **Interactive Chatbot**: Real-time chat interface to communicate with a chatbot, styled for user and AI responses.
- **Image Generation**: Generate images based on user-provided prompts.
- **Dynamic Switching**: Easily switch between chatbot and image generator functionalities using the navigation bar.
- **Real-time WebSocket Communication**: Chat responses are streamed in real-time.

## Project Structure

```plaintext
.
├── main.py               # Main FastAPI application
├── templates/            # HTML templates
│   ├── home.html         # Chatbot interface
│   ├── image.html        # Image generation interface
│   ├── layout.html       # Base layout for all pages
│   ├── navbar.html       # Navigation bar
├── requirements.txt      # Python dependencies
├── .env                  # Environment variables
└── README.md             # Project documentation


Installation
Follow these steps to set up the project locally:

Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Set Up a Virtual Environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies:

bash
Copy code
pip install -r requirements.txt
Set Environment Variables: Create a .env file in the project root and add your OpenAI API key:

plaintext
Copy code
OPENAI_API_SECRET_KEY=your_openai_api_key
Run the Application:

bash
Copy code
uvicorn main:app --reload
Access the Application: Open your browser and navigate to http://127.0.0.1:8000.

Usage
Chatbot
Navigate to the Chatbot page.
Enter your message in the input field and click Send.
View the chatbot's real-time responses in the chat history.
Image Generator
Navigate to the Image Generator page.
Enter a prompt describing the desired image and click Send.
View the generated image below the input field.
Technologies Used
Backend: FastAPI
Frontend: HTML, Jinja2, Bootstrap
API: OpenAI (GPT-4 and DALL·E)
WebSocket: Real-time communication
Environment Management: python-dotenv
File Details
main.py
Contains route definitions for both chatbot and image generator functionalities.
Handles WebSocket connections for streaming chat responses.
Integrates OpenAI API for GPT-4 and DALL·E.
Templates
layout.html: Base template with reusable styles and scripts.
home.html: Chat interface for user and AI messages.
image.html: Image generation interface.
requirements.txt
Dependencies for the project:

plaintext
Copy code
aiofiles==24.1.0
fastapi==0.115.0
Jinja2==3.1.3
openai==1.30.1
python-dotenv==1.0.1
python-multipart==0.0.12
uvicorn==0.31.1
websockets==14.1
Future Improvements
Persist Chat History: Save conversations in a database or local storage for future reference.

Improved Image Display: Enhance the UI for displaying generated images.

Error Handling: Provide user-friendly messages for API errors or WebSocket disconnections.

Customizable Chatbot Personalities: Allow users to select from different AI personalities or behavior types.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgments
OpenAI for providing GPT-4 and DALL·E APIs.
FastAPI for building a robust backend.
Bootstrap for frontend styling.
vbnet
Copy code

