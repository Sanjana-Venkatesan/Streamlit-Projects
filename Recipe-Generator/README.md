# Recipe Generator

The **Recipe Generator** is a Streamlit-based web app that helps users create personalized recipes based on their preferences, available ingredients, and allergies. The app uses Google's Generative AI to suggest recipes that align with the user's specific needs and dietary requirements.

## Features

- **Ingredient Input**: Users can input a list of available ingredients.
- **Dietary Preference Selection**: Users can specify their dietary preference (vegetarian, non-vegetarian, or vegan).
- **Allergy Information**: Users can mention any allergies to avoid ingredients in the generated recipe.
- **AI-Powered Recipe Generation**: The app uses Google's Generative AI model to suggest suitable recipes based on the user's input.

## Requirements

Before running the app, make sure to install the following Python libraries:

- `streamlit`: For the web app interface.
- `google-generativeai`: For interacting with Google's Generative AI model.

You can install these dependencies by running:

```bash
pip install streamlit google-generativeai
```

## Setup

1. **API Key**: The app uses Google's Generative AI, which requires an API key. To obtain an API key, visit [Google Cloud AI](https://cloud.google.com/ai) and create a project to generate the API key.
   - Once you have the API key, replace the placeholder in the code with your own API key: 
   ```python
   genai.configure(api_key="YOUR_API_KEY")
   ```

2. **Run the App**:
   After setting up the API key, run the app with the following command:

   ```bash
   streamlit run app.py
   ```

3. **Access the App**:
   Open the provided local URL in your browser to interact with the app.

## How It Works

1. **Enter Ingredients**: Users enter a list of ingredients they have available.
2. **Select Dietary Preference**: Users select their dietary preference (vegetarian, non-vegetarian, or vegan).
3. **Provide Allergy Information**: Users mention any allergies to avoid in the recipe.
4. **Generate Recipe**: The app sends the inputs to Google's Generative AI model, which generates a recipe based on the user's preferences and constraints.
5. **Display Recipe**: The app returns and displays the generated recipe.

## Example Use Cases

- **Generate Recipes**: Enter the ingredients you have in your kitchen and get a recipe suggestion based on your dietary preference.
- **Avoid Allergies**: Specify ingredients you're allergic to, and the app will ensure the generated recipe avoids them.
- **Personalized Cooking**: Whether you're vegetarian, vegan, or non-vegetarian, the app can suggest a recipe tailored to your needs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
