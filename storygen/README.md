# Story Generator App

This app generates personalized stories for children based on their reading level, interests, and character selection. The app uses Google's Gemini API to generate content based on user inputs.

## Features

- **Child Profile Setup**: Allows users to select a reading level, input their child's interests, and choose a favorite character.
- **Personalized Story Generation**: Generates a child-friendly story based on the selected parameters.
- **Story Interaction**: Users can request a new story or stop listening at any time.

## Prerequisites

Ensure the following dependencies are installed:

- Python 3.x
- Streamlit
- Pillow
- Requests
- Google Generative AI (gemini-pro)

### Install dependencies

```bash
pip install streamlit pillow requests google-generativeai
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

4. Open your browser and go to `http://localhost:8501` to use the story generator.

## How It Works

1. **User Profile Setup**:
   - The user selects a reading level for the child (e.g., "Preschool", "Elementary (K-2)", "Elementary (3-5)").
   - The user provides a list of the child's interests (e.g., "space, adventure").
   - The user selects a favorite character from a list (e.g., "Twinkle", "Maya", "Tia", "Lily").

2. **Story Generation**:
   - The selected inputs are sent to the **Google Gemini API** to generate a personalized story prompt.
   - The **Gemini Model** generates a story based on the prompt and returns the story content.

3. **Story Interaction**:
   - The user can request a new story or stop listening at any time.

## Google Gemini API Integration

The app interacts with the **Google Gemini API** for story generation using the following code:

```python
genai.configure(api_key="Your-API-Key")
model = genai.GenerativeModel(model_name="gemini-pro")

story_segment = model.generate_content(prompt)
```

Ensure that you replace `"Your-API-Key"` with your actual **Google Gemini API key**.

## Customization

- **Character Images**: The app uses pre-defined character images. You can add more characters and images by updating the `characters` dictionary with additional links.
- **Reading Levels & Interests**: You can customize the available reading levels and the way interests are handled by adjusting the list of `reading_level_options` and modifying the interest input processing.

## License

This project is licensed under the **MIT License**.
