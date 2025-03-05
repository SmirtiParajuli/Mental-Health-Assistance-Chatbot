********** Mental-Health-Assistance-Chatbot **********

A conversational AI chatbot designed to provide empathetic mental health support using Large Language Models (LLMs) and Natural Language Processing (NLP).

📌 Project Overview

The Mental Health Assistance Chatbot is an AI-powered virtual assistant designed to provide empathetic and contextually relevant support to individuals seeking mental health guidance. Built using OpenAI’s GPT-3.5 Turbo, Natural Language Processing (NLP), and Speech Recognition, this chatbot simulates counseling conversations to assist users in expressing their thoughts and emotions in a safe and accessible manner. Mental health concerns are often met with barriers such as stigma, financial constraints, and limited access to professional services. This project aims to bridge that gap by offering a scalable, anonymous, and cost-effective mental health support system.
         
This chatbot is not a replacement for professional therapy but serves as a first-line intervention for individuals seeking anonymous and accessible mental health support

🎯 Features & Capabilities

         -> Conversational AI - Utilizes GPT-3.5 Turbo (fine-tuned) for intelligent responses.
         -> Speech Recognition - Users can interact via voice input instead of typing.
         -> Text-to-Speech (TTS) - AI-generated responses are spoken aloud for a more human-like experience.
         -> Graphical Interface (GUI) - Simple Tkinter-based GUI to display conversations.
         -> Conversation Saving - Users can download & review past chatbot interactions.
         -> Privacy Focused - Does not store user data; conversations are temporary.
         
🛠️ Technologies Used

         -> AI Model - OpenAI GPT-3.5 Turbo (Fine-Tuned)
         -> NLP Processing	- Python, OpenAI API
         -> Speech Recognition - speech_recognition Library
         -> Text-to-Speech (TTS) - pyttsx3 Library
         -> Graphical Interface - Tkinter (Python GUI)
         -> Data Processing - Pandas, JSON

📁 Dataset

 Mental Health Counseling Conversations Dataset (Hugging Face)
 
                    - 3,500+ counseling interactions between individuals and psychologists
                    - Sourced from two online therapy platforms
                    - Structured in JSON format
                    - Anonymized & cleaned for ethical AI use


🚀 How to Run the Chatbot Locally
   1️⃣ Clone the Repository
   
            git clone <repository-url> 
            cd Mental-Health-Chatbot
 
   2️⃣ Set Up a Virtual Environment (Recommended)
         
         python -m venv venv
         source venv/bin/activate  # On Mac/Linux
         venv\Scripts\activate     # On Windows
         
   3️⃣ Install Dependencies

            pip install -r requirements.txt

   4️⃣ Set Up OpenAI API Key
   
      -> Create an .env file in the project root.
      -> Add your OpenAI API key:
           OPENAI_API_KEY="your_api_key_here"

   5️⃣ Run the Chatbot

📝 Usage Instructions

         1️⃣ Open the chatbot GUI.
         2️⃣ Speak or type your message.
         3️⃣ The chatbot will generate a response and read it aloud.
         4️⃣ Conversations are displayed in the GUI.
         5️⃣ Users can save their chat history for later review.


🔬 Model Training & Fine-Tuning Process

  Dataset Used
  
         -> Mental Health Conversations Dataset from Hugging Face
         -> Contains 3,500+ real counseling sessions (fully anonymized).
         -> Preprocessed using NLP techniques (lowercasing, punctuation removal, stopwords filtering).

  Fine-Tuning on GPT-3.5 Turbo
  
         -> Data formatted as JSONL.
         -> Uploaded to OpenAI for fine-tuning:

                  openai.FineTuningJob.create(
                      training_file="dataset.jsonl",
                      model="gpt-3.5-turbo"
                  )
                  
  Speech Processing & TTS     
  
              -> speech_recognition used for speech-to-text.
              -> pyttsx3 used for text-to-speech AI responses.       


📊 Performance & Limitations

✅ Strengths:

         ✔️ Provides empathetic and meaningful responses.
         ✔️ Supports speech-based interaction, making it accessible.
         ✔️ Works well for common mental health concerns (anxiety, grief, motivation).
         ✔️ Lightweight Tkinter-based GUI for easy usability.

⚠️ Limitations:

         ❌ May generate generic responses for complex mental health conditions.
         ❌ Requires internet access for API calls.
         ❌ Limited accuracy in handling speech recognition errors.
         ❌ Not a replacement for licensed therapy professionals.

🔮 Future Enhancements

         🚀 Improve Speech Recognition – Fine-tune model to handle accent variations & background noise.
         🚀 Context-Aware Responses – Enable chatbot to track longer conversations.
         🚀 Sentiment Analysis – Adjust chatbot tone based on user emotional state.
         🚀 Mobile App Version – Implement chatbot as a cross-platform mobile application. 

💼 Contributors

            Smriti Parajuli	AI Model Implementation & NLP Processing
            Gloria Hawkins-Roberts 	GUI & Speech Processing Development

📜 License

  This project is for educational and research purposes only. Do not use it as a substitute for professional mental health services.
