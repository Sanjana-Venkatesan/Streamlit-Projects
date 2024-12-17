# Text to Image Chatbot using Stable Diffusion

This is a **Streamlit-based chatbot** that utilizes the **Stable Diffusion XL model** from Hugging Face to generate images from user prompts. The chatbot listens to the user's input, sends it to the model, and then responds with a generated image based on the prompt.

## Features

- **Text to Image Generation**: Converts text prompts into images using Stable Diffusion XL.
- **Chat Interface**: A simple chat-based interface where users can interact with the chatbot and view the generated images.
- **Stable Diffusion API Integration**: Utilizes the Hugging Face Inference API for generating images.

## Prerequisites

Ensure the following dependencies are installed:

- Python 3.x
- Streamlit
- Requests
- Pillow (PIL)

### Install dependencies

```bash
pip install streamlit requests pillow
```

## Setup and Running the Application

1. **Clone or create the app**: Copy the script into your project directory.
2. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

3. Open your browser and go to `http://localhost:8501` to use the chatbot.

## How It Works

1. **User Input**: The user types a prompt into the chat input field (e.g., "a working woman").
2. **Text to Image Conversion**: The prompt is sent to the **Stable Diffusion XL** model via the Hugging Face Inference API. 
3. **Image Generation**: The model generates an image based on the prompt and returns the image bytes.
4. **Displaying the Image**: The generated image is displayed in the chat interface alongside the assistant's message.

## API Integration

The app communicates with the **Stable Diffusion XL model** hosted on Hugging Face through the following API:

```python
API_URL = "https://api-inference.huggingface.co/models/stabilityai/stable-diffusion-xl-base-1.0"
response = requests.post(API_URL, headers=headers, json=payload)
```

The `headers` include the Hugging Face API token, and the `payload` contains the text prompt.

### API Key

Ensure you replace the `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` API key with your own Hugging Face API key. You can obtain an API key by creating an account on Hugging Face and subscribing to their Inference API.

## Customization

- You can adjust the design and functionality to improve user experience, such as customizing the chat interface or adding additional image generation settings.
- Change the model URL if you want to use a different model hosted on Hugging Face.

## License

This project is licensed under the **MIT License**.
