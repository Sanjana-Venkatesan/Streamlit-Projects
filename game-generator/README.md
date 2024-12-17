# Game Crew Task Management Application

This application helps manage tasks related to game development using **CrewAI** and **Streamlit**. It involves multiple AI agents who work together to build, review, and evaluate a Python game based on the input provided by the user.

## Features

- **Game Development Process**:
  - **Senior Software Engineer**: Responsible for writing the game code based on the provided game description.
  - **Software Quality Control Engineer**: Reviews the code, checks for syntax errors, missing imports, and potential vulnerabilities.
  - **Chief Software Quality Control Engineer**: Evaluates the final game code to ensure it meets the required standards and functionality.

- **Generative AI**: Uses **Google Gemini** (via `langchain_google_genai`) to assist agents in generating and evaluating code.

- **Streamlit Interface**: Provides an easy-to-use web interface for users to input their game requirements and receive the final game code.

## Prerequisites

To run this application, ensure you have the following dependencies installed:

- Python 3.x
- Streamlit
- CrewAI
- langchain_google_genai
- Google API Key (for Google Generative AI)

Install the dependencies using pip:

```bash
pip install streamlit crewai langchain_google_genai
```

## Setup

1. **Clone the repository** (or create a new file) and copy the script into your local directory.
2. **Set up your Google API Key**:
   - Get your **Google API Key** from the [Google Cloud Console](https://console.cloud.google.com/).
   - Replace `YOUR_GOOGLE_API_KEY` in the script with your actual API key.
   
3. **Run the Streamlit App**:
   - Once the setup is complete, open a terminal and navigate to your project directory.
   - Run the Streamlit app by executing the following command:
   
   ```bash
   streamlit run app.py
   ```

4. Open your browser and go to `http://localhost:8501` to interact with the application.

## How It Works

1. **Input**:
   - The user enters a description of the game they want to create, including game mechanics and any specific requirements.
   
2. **Task Management**:
   - The app manages three key tasks:
     - **Code Task**: The Senior Software Engineer creates the game code.
     - **Review Task**: The QA Engineer checks the code for errors.
     - **Evaluation Task**: The Chief QA Engineer evaluates the code for completion and quality.

3. **Output**:
   - The final game code is generated and displayed in the app.

## Example Use Case

1. Open the app in your browser.
2. Enter the game details (e.g., game mechanics, story, etc.).
3. Click "Run".
4. The app will generate the Python code for your game, review it for errors, and evaluate its functionality.
5. The final code will be displayed in the app.

## Customization

- You can modify the agents' backstories and tasks to adapt to different project types or game genres.
- You can also integrate more sophisticated agents or models depending on the complexity of the game you're working on.

## Contributing

Feel free to contribute to this project by forking the repository and submitting pull requests for improvements or bug fixes.

## License

This project is licensed under the MIT License.
