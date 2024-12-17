# Book Recommendation App

This app provides book recommendations based on text analysis using the Google Gemini API. Users input a text, and the app analyzes the text to suggest books that align with the user's current situation or mood.

## Features

- **Text Input**: Users provide a text (e.g., a sentence or short paragraph) that represents their current situation or mood.
- **Book Recommendation**: The app analyzes the provided text and recommends a book that aligns with the user's emotions or state of mind.
- **Explanation**: The app provides a short explanation of why the recommended book was chosen based on the input text.

## Prerequisites

Ensure the following dependencies are installed:

- Python 3.x
- Streamlit
- Google Generative AI (gemini-pro)

### Install dependencies

```bash
pip install streamlit google-generativeai
```

## Setup and Running the Application

1. **Clone or create the app**: Copy the script into your project directory.
2. **Get the API Key**: You will need a **Google Gemini API key**. You can generate this key in your Google Cloud console and configure it in the app as shown below:
    ```python
    genai.configure(api_key="Your-API-Key")
    ```
3. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

4. Open your browser and go to `http://localhost:8501` to use the book recommendation app.

## How It Works

1. **User Input**: The user enters a text in the input field that reflects their current mood or situation.
2. **Text Analysis**: The app sends this text to the **Google Gemini API** to analyze it and determine what type of book would suit the user.
3. **Book Recommendation**: Based on the text analysis, the app generates a book recommendation and provides a brief explanation of why that particular book is recommended.

## Google Gemini API Integration

The app uses the **Google Gemini API** to generate book recommendations with the following code:

```python
genai.configure(api_key="Your-API-Key")
llm = genai.GenerativeModel(model_name="gemini-pro")

human_prompt = prompt(text)
response = llm.generate_content(human_prompt)
```

Ensure that you replace `"Your-API-Key"` with your actual **Google Gemini API key**.

## Customization

- **Prompt Customization**: You can adjust the prompt template to change how the app interprets the user’s input or modify the book recommendation process.
- **Text Analysis Logic**: You can modify the `prompt` function to analyze different aspects of the text or focus on specific moods or themes to generate more specific recommendations.

## License

This project is licensed under the **MIT License**.
