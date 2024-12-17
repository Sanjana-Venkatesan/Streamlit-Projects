# Novel Prologue & Epilogue Generator

This Streamlit application helps you generate the prologue and epilogue of a novel based on user-provided details such as the novel's name, genre, and protagonists. The app uses Google’s Generative AI API to create unique, human-like prologues and epilogues, complete with witty dialogues, descriptions, and character points of view.

## Features

- **Novel Title**: Input the title of your novel.
- **Genre**: Enter the genre(s) of the novel (e.g., fantasy, romance, mystery).
- **Protagonists**: Provide a brief description of the protagonists (character names and descriptions).
- **Prologue and Epilogue Generation**: Automatically generates a prologue and epilogue based on the provided details.
- **Human-like Content**: The generated content includes witty remarks, character descriptions, and dialogue, all from the point of view of the characters.

## Requirements

Ensure you have the following Python libraries installed:

- **Streamlit**: For creating the web interface.
- **Google Generative AI**: For generating the prologue and epilogue text.
- **Google Cloud API Key**: You’ll need to configure the Google Cloud API with your own API key.

To install the required libraries, run:

```bash
pip install streamlit google-generativeai
```

## Setup

1. **Obtain Google API Key**:
   - You’ll need an API key from Google to use the Generative AI model. Ensure your API key is valid and has access to the necessary AI services.

2. **Install the Required Libraries**:
   If you haven’t already, install the necessary libraries using the command mentioned above.

3. **Run the App**:
   Save the Python script as `novel_prologue_epilogue_generator.py` (or any name you prefer), and run the following command:

   ```bash
   streamlit run novel_prologue_epilogue_generator.py
   ```

   This will launch the application in your default browser.

## How It Works

1. **Enter Details**:
   - Provide the **Novel Name**, **Genre**, and **Protagonist Descriptions** in the respective fields.

2. **Generate Prologue & Epilogue**:
   - After entering the details, click on the "Generate Prologue & Epilogue" button.
   - The app will send a request to the Google Generative AI model to generate the content based on your inputs.

3. **View Results**:
   - Once the content is generated, the prologue and epilogue will be displayed separately on the screen. The prologue will appear first, followed by the epilogue.

4. **Character Point of View**:
   - The prologue and epilogue will be written from the point of view of the characters, with witty dialogue and descriptive elements to make the story engaging.

## Example Usage

- **Novel Name**: *The Lost Kingdom*
- **Genre**: *Fantasy, Adventure*
- **Protagonists**: *Arthur, a brave knight; Seraphina, a mysterious sorceress*

The application will generate a prologue that sets the stage for the story and an epilogue that wraps up the events after the main story concludes, both full of character-driven dialogue and engaging narrative.

## File Structure

- **novel_prologue_epilogue_generator.py**: The main Python script that runs the Streamlit app.
- **requirements.txt**: (Optional) A list of required libraries, which can be installed using `pip install -r requirements.txt`.

## License

This project is open-source and can be used and modified freely for personal or educational purposes. For commercial use, please ensure compliance with the necessary licenses of third-party libraries used.
