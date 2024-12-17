# Chatbot with Gemini AI Integration

This is a chatbot application built using **Streamlit** and **Google's Generative AI (Gemini)**. It enables users to interact with a chatbot that responds in real-time, saves conversation history, and allows users to pick past chats for further interactions.

## Features

- **Interactive Chat**: The chatbot interacts with users in real-time using **Google Gemini API** for generating responses.
- **Persistent History**: It stores previous chat sessions in local storage, allowing users to select and continue from where they left off.
- **Message Display**: Messages are displayed with the role of the sender (user or AI), and each response is shown incrementally, making it look like the AI is typing.
- **Chat Session Management**: Users can switch between different chat sessions and pick from a list of past conversations.
  
## Requirements

Before you run this application, ensure you have the following libraries installed:

- **Streamlit**: For creating the web app.
- **Google Generative AI (Gemini)**: For generating chatbot responses.
- **Joblib**: For serializing and saving conversation data.
- **Other dependencies**: `os`, `time`, etc.

Install the required libraries using the following command:

```bash
pip install streamlit google-generativeai joblib
```

## Setup

1. **Google API Key**: The script requires a valid Google API key for interacting with the Gemini model. Replace the placeholder `AIzaSyDKcxALky8LiROaxb0RGMw8TLLOcujMRMY` in the `genai.configure` function with your actual API key.
   
2. **Storage Directory**: The app stores conversation data locally in a `data/` folder. This folder is created automatically on the first run, but if needed, you can create it manually. This directory will store:
   - `past_chats_list`: A list of all chat sessions.
   - `{chat_id}-st_messages`: A file containing all user and AI messages for a particular session.
   - `{chat_id}-gemini_messages`: A file containing historical chat data required by the Gemini model.

## Running the App

To run the chatbot app, use the following command:

```bash
streamlit run <filename>.py
```

Replace `<filename>` with the name of your script file.

### User Interface

- **Sidebar**: Displays the history of past chat sessions. Users can pick from a list of past chats or start a new one.
- **Chat Window**: The main interface where the conversation takes place. The user can input messages, and the chatbot responds with real-time generated text.
  
### How It Works

1. **New Chat Session**:
    - The first time you use the app, it creates a new chat session with an empty history.
    - The user can interact with the chatbot by typing messages into the chat window. The chatbot will respond with generated text from the Gemini model.

2. **Chat History**:
    - When a user sends a message, the conversation history is saved to the local disk. This includes both the user's inputs and the model's responses.
    - The next time the user visits the app, they can choose to continue from the previous chat or start a new chat.
    - The session is saved with a unique `chat_id` and `chat_title`.

3. **Message Flow**:
    - For each message the user sends, the chatbot responds in chunks with a delay between them to simulate typing.
    - The full response is displayed once the message is fully generated.

4. **Selecting Past Chats**:
    - If the user has interacted with the chatbot before, they can select a past chat session from the sidebar and continue where they left off.
    - This allows users to maintain a continuous conversation over multiple sessions.

5. **Saving Chat Data**:
    - The chatbot saves conversation data in a folder called `data/` as serialized files. These files contain both the user inputs and AI-generated responses for each chat session.
  
## Files and Directories

- **data/**: Contains serialized files storing chat history and metadata.
- **past_chats_list**: Stores the list of chat sessions.
- **{chat_id}-st_messages**: Contains the messages exchanged between the user and the chatbot.
- **{chat_id}-gemini_messages**: Contains the raw conversation history needed for the Gemini model.

## Notes

- **API Key**: Make sure that your Google API key is valid and has access to Gemini models.
- **Local Storage**: This app uses local storage (on the user's machine) to store chat data. It assumes the app is running in an environment where the filesystem is accessible.
- **Chat Persistence**: Since chat sessions are saved locally, ensure that you maintain backup copies of the data if you intend to use the app on multiple machines or environments.

## License

This project is open-source and can be modified for personal or educational use. For commercial use, ensure compliance with Google's API usage policies.
