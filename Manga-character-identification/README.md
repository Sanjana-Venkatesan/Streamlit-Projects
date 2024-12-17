# Manga Character Identification

This Streamlit app allows users to upload an image or provide an image URL of a manga character, and it will identify the character, their role, and the manga or manhua they are from. The app uses Google's Generative AI API to analyze the image and generate a detailed response based on the character's features.

## Features

- **Upload Image**: Users can upload images in JPG, JPEG, or PNG formats.
- **Enter Image URL**: Users can enter an image URL, and the app will fetch and analyze the image.
- **Manga Character Identification**: The app uses a generative AI model to identify the character in the image, determine which manga/manhua they are from, and describe their role in the story.
- **Image Display**: The uploaded or fetched image is displayed with a caption.

## Requirements

Before running the app, ensure you have the following Python libraries installed:

- `streamlit`: For the web app interface.
- `PIL`: For handling image uploads and processing.
- `requests`: For fetching images from URLs.
- `google-generativeai`: For interacting with the Google Generative AI API.

You can install these dependencies by running:

```bash
pip install streamlit Pillow requests google-generativeai
```

## Setup

1. **API Key**: To use the Google Generative AI API, you'll need an API key. Replace the placeholder in the code with your own API key.
   - You can obtain an API key from [Google Cloud AI](https://cloud.google.com/ai).

2. **Run the App**:
   After setting up the API key, run the app with the following command:

   ```bash
   streamlit run app.py
   ```

3. **Access the App**:
   Open the provided local URL in your browser to interact with the app.

## How It Works

1. **Input Options**: 
   - You can upload an image directly or provide the URL of an image.
   - The app will fetch and process the image from the URL or the uploaded file.

2. **Manga Character Identification**: 
   - Once an image is provided, the app uses the Google Generative AI model to identify the character, determine the manga/manhua they are from, and describe their role.
   - The result is displayed as text below the image.

## Example Use Cases

- **Upload Image**: Upload a picture of your favorite manga character, and the app will tell you who they are and which manga/manhua they belong to.
- **Enter Image URL**: If you have a URL to an image, simply paste it, and the app will identify the character.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
