# Quizbee_chatbot
QuizBee — Local CLI Chatbot using Hugging Face LLM

#  QuizBee CLI Chatbot

A lightweight, instruction-following chatbot powered by [TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0). Run entirely from your terminal — no GPU required!

---

##  Features

-  Runs entirely on CPU — no disk offloading or GPU needed
-  CLI chatbot with loading animation and memory context
-  Clean prompt formatting and friendly interaction
-  Lightweight model for fast startup and low memory

---

##  Folder Structure

ChatBot/ 

├── chat_memory.py # Sliding conversation memory buffer 

├── model_loader.py # Loads and returns the chatbot pipeline 

├── interface.py # Terminal-based chatbot loop 

├── requirements.txt # Python dependencies 

├── README.md # This file 


---

## Setup Guide


1. Clone the Repo / Unzip Folder

git clone [repo_link] && cd quizbee_chatbot

2. Set Up Virtual Environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

3. Install Dependencies
pip install -r requirements.txt

4. Run the Chatbot
python interface.py

Demo Starts:
💬 Chatbot is ready! Type your message below. Type /exit to quit.
You: What is the capital of Canada?
Bot: The capital of Canada is Ottawa.
You: Brazil?
Bot: The capital of Brazil is Brasilia.
You: /exit
Exiting chatbot. Goodbye!


## Notes
- You can customize the behavior by editing the system instruction inside interface.py

- If a user types only a country name, the bot will still try to infer intent thanks to prompt design

- This model does not support memory recall across sessions

## Requirements
- Python 3.8 or higher

- transformers >= 4.39.0

- torch >= 2.1.0

- accelerate >= 0.27.2

Runs on Windows, Linux, and macOS — no GPU required.


## License
This project is licensed under the MIT License — feel free to remix and expand.

Video Link : https://drive.google.com/file/d/1BZR-JByNsVYF_nfZVWq28eUQfV2OdVLA/view?usp=drive_link

## Demo PDF
The PDF used in the demo video is available in the repository:

It includes:

Project architecture

Key features

Sample interaction

Setup steps

