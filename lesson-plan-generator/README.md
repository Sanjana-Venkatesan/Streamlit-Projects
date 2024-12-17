
# Craft Lesson Plan Generator

This is a **Streamlit-based application** designed to assist teachers in crafting lesson plans. By entering a subject, topic, and duration, the app generates a detailed lesson plan using the power of **Google Generative AI (Gemini Pro)**.

## Features

- **Lesson Plan Generation**: The app generates comprehensive lesson plans, including learning objectives, engaging activities, and assessment strategies, based on the given subject, topic, and duration.
  
- **Google Generative AI**: Utilizes Google Gemini Pro for generating human-like lesson plans tailored to the input parameters.

- **Interactive Streamlit Interface**: Provides an easy-to-use web interface where users can input the necessary details and generate lesson plans with a single click.

## Prerequisites

To run this application, you need to have the following dependencies:

- Python 3.x
- Streamlit
- google-generativeai

### Install the required dependencies

```bash
pip install streamlit google-generativeai
```

## Setup

1. **Clone the repository** (or create a new file) and copy the script into your local directory.

2. **Set up your Google API Key**:
   - Get your **Google API Key** from the [Google Cloud Console](https://console.cloud.google.com/).
   - Replace `<api>` in the script with your actual API key.

3. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to launch the app:
   
   ```bash
   streamlit run app.py
   ```

4. Open your browser and go to `http://localhost:8501` to interact with the app.

## How It Works

1. **Input**: 
   - Enter the **subject**, **topic**, and **duration** for which you want to generate a lesson plan.

2. **Generate Lesson Plan**: 
   - Upon clicking the "Generate Lesson Plan" button, the app sends a request to Google Generative AI and generates a detailed lesson plan for the provided parameters.

3. **Output**: 
   - The generated lesson plan is displayed, including learning objectives, suggested activities, and assessment strategies.

## Example Use Case

1. Open the app in your browser.
2. Fill in the subject (e.g., "Math"), topic (e.g., "Algebra"), and duration (e.g., "1 hour").
3. Click "Generate Lesson Plan".
4. The app will generate a lesson plan that includes structured teaching steps, objectives, and assessment strategies.
5. Review the generated lesson plan and adapt it for your classroom needs.

## Customization

- The app can be customized to handle different formats, including specific sections for learning outcomes, material lists, and any other teaching resources you need to include.
- You can integrate additional AI models or adapt the prompt template for specific educational settings.

## Contributing

Feel free to contribute to this project by forking the repository and submitting pull requests for improvements, additional features, or bug fixes.

## License

This project is licensed under the MIT License.
