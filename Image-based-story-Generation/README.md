# Image-Based Storytelling with Language Model

This Streamlit app allows users to generate a cohesive story based on a sequence of images. The app uses a powerful generative language model from Langchain and Google Generative AI to create a narrative that links the provided images together. Users can either upload images or provide image URLs, and the app will generate a story that connects the context of the images.

## Features

- **Upload Images**: Users can upload multiple images (JPG, JPEG, PNG) and the app will create a story based on these images.
- **Enter Image URLs**: Users can input URLs of images, and the app will fetch and use these images to generate a story.
- **Story Generation**: Once images are uploaded or URLs are provided, the app generates a cohesive story that connects the sequence of images.

## Requirements

Before running this app, ensure you have the following Python libraries installed:

- `streamlit`: For the web app interface.
- `PIL`: For image handling.
- `requests`: To fetch images from URLs.
- `langchain_google_genai`: For interacting with Google's generative AI API.
- `IPython`: For Markdown support.
- `textwrap`: For formatting text.

You can install these dependencies by running:

```bash
pip install streamlit Pillow requests langchain_google_genai IPython textwrap
```

## How to Run

1. Clone this repository to your local machine or open the script in your preferred IDE.
2. Install the required dependencies listed above.
3. Run the app using Streamlit:

```bash
streamlit run app.py
```

4. Open the provided local URL in your browser to interact with the app.

## How It Works

- **Input Options**: Choose between uploading images or entering image URLs. The app supports multiple image uploads.
- **Story Generation**: Once images are provided, the app sends them to the Langchain-based language model to generate a cohesive story that links the images.
- **Displaying Results**: The generated story is displayed under an expandable section.

## API Key

The app uses Google's generative AI through the `langchain_google_genai` library. To use the app, you need to replace the `google_api_key` in the code with your own API key.

You can obtain an API key by visiting [Google Cloud's AI Services](https://cloud.google.com/ai).

## Example

1. Upload a sequence of images.
2. Click on the "Generate Story" button.
3. View the generated story that links your images together.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
