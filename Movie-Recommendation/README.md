# Movie Recommendation App

The **Movie Recommendation App** is a Streamlit-based application that provides movie recommendations similar to a given movie. The app uses Google's Generative AI to analyze the input movie and generate a list of similar films, along with explanations for why each recommendation is relevant.

## Features

- **Movie Name Input**: Enter the name of a movie you want to get recommendations for.
- **AI-Powered Recommendations**: The app generates five movie recommendations based on the given movie using Google's Generative AI.
- **Explanations**: For each recommended movie, the app provides an explanation of why it is similar to the original movie.
- **Dynamic Styling**: Each recommendation is displayed with random background colors and text styling for a personalized look.

## Requirements

Before running the app, ensure you have the following Python libraries installed:

- `streamlit`: For the web app interface.
- `google-generativeai`: For interacting with Google's generative AI model.
- `IPython`: For Markdown support.
- `textwrap`: For formatting text.
- `random`: For random color generation in the UI.

You can install these dependencies by running:

```bash
pip install streamlit google-generativeai IPython textwrap
```

## Setup

1. **API Key**: The app uses Google's Generative AI, which requires an API key. To obtain an API key, visit [Google Cloud AI](https://cloud.google.com/ai) and create a project to generate the API key.
   - Once you have the API key, replace the placeholder in the `genai.configure(api_key='YOUR_API_KEY')` with your own API key.

2. **Run the App**:
   After setting up the API key, you can run the app with the following command:

   ```bash
   streamlit run app.py
   ```

3. **Access the App**:
   Open the provided local URL in your browser to interact with the app.

## How It Works

1. **Enter Movie Name**: The user enters the name of a movie they want recommendations for.
2. **AI Processing**: The app sends the movie name to the Google Generative AI model, which then generates a list of five similar movies and provides an explanation for each.
3. **Display Recommendations**: The app displays the recommendations in a visually distinct style with random background colors and formatted explanations.

## Example Use Cases

- **Enter a Movie Name**: Type the name of a movie you like, and the app will recommend similar movies that match its theme, genre, or storyline.
- **Recommendations**: The app will return a list of five movies with explanations, making it easier to discover new films.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
