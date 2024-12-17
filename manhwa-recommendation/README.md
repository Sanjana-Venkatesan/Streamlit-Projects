# Manhwa Recommendation App

This is a **Streamlit-based web application** that recommends manhwas based on user preferences. The app uses **Google Generative AI (Gemini Pro)** to generate personalized manhwa recommendations based on your favorite manhwa, preferred genres, pacing, romance preferences, and themes.

## Features

- **Personalized Manhwa Recommendations**: The app generates five manhwa recommendations based on the user’s input preferences and their favorite manhwa.
- **Manhwa Synopsis**: Provides a brief synopsis of the user’s favorite manhwa.
- **AI-Powered**: Uses Google Generative AI (Gemini Pro) to generate recommendations and synopses.
- **Streamlit UI**: User-friendly interface for easy interaction with the application.

## Prerequisites

Before running the application, ensure that you have the following dependencies:

- Python 3.x
- Streamlit
- google-generativeai

### Install the required dependencies

```bash
pip install streamlit google-generativeai
```

## Setup

1. **Clone or create the app**: Copy the script into your local directory.
2. **Set up your Google API Key**:
   - Obtain your **Google API Key** from the [Google Cloud Console](https://console.cloud.google.com/).
   - Replace `<api key>` in the script with your actual API key.
3. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

4. Open your browser and go to `http://localhost:8501` to use the app.

## How It Works

1. **Input**:
   - Enter the name of your **favorite manhwa**.
   - Answer a series of questions about your **preferred genre**, pacing, romance preferences, and themes you enjoy.

2. **Generate Recommendations**:
   - Click the "Get Recommendations" button, and the app sends a request to **Google Generative AI** to generate a personalized set of five manhwa recommendations based on your preferences.

3. **Output**:
   - The app displays:
     - A brief **synopsis** of your favorite manhwa.
     - Five manhwa recommendations with an explanation of why each one is similar to your favorite.

## Example Use Case

1. Open the app in your browser.
2. Enter your **favorite manhwa's title**.
3. Answer the questions about your **preferences**.
4. Click "Generate Recommendations".
5. Review the generated **synopsis** and **five recommendations**.
6. Each recommendation is explained in terms of how it aligns with your preferences.

## Customization

You can customize this app in various ways:
- **Add More Questions**: If you want to collect more specific preferences from the user, you can add additional questions.
- **Improve the Prompt**: Modify the AI prompt to provide more detailed or varied recommendations.
- **Modify Output**: Tailor the format of the recommendations or display them differently.

## Contributing

Feel free to fork the repository and submit pull requests for bug fixes, improvements, or new features.

## License

This project is licensed under the **MIT License**.
