# Text Extraction from Images

The **Text Extraction from Images** web application allows users to extract text from images using Optical Character Recognition (OCR). The app supports both uploading an image directly or providing an image URL. It utilizes **EasyOCR** for text detection and extraction from the image content.

## Features

- **Upload Image**: Upload an image directly from your local machine to extract text.
- **Image URL**: Provide an image URL, and the app will fetch the image to extract the text.
- **Text Extraction**: Extracted text from the image will be displayed in the app for review.
- **Supports Various Image Formats**: The app supports image formats such as JPG, PNG, and JPEG.
  
## Requirements

Before running the app, make sure to install the following dependencies:

- `streamlit`: For building the web app interface.
- `opencv-python`: For image processing and manipulation.
- `Pillow`: For image loading and manipulation.
- `easyocr`: For extracting text from images using OCR.
- `requests`: For handling image URLs.

Install the required dependencies using `pip`:

```bash
pip install streamlit opencv-python Pillow easyocr requests
```

## Setup

1. **Run the App**: After installing the dependencies, run the following command to launch the app:

   ```bash
   streamlit run app.py
   ```

2. **Access the App**: Open the provided local URL in your browser to interact with the app.

## How It Works

1. **Upload Image**: Users can upload an image directly from their computer.
2. **Provide Image URL**: Users can enter the URL of an image hosted on the web.
3. **Extract Text**: The app processes the image and extracts the text using EasyOCR, displaying the results on the screen.
4. **Error Handling**: If no text is detected, or if the image cannot be processed, the app provides an appropriate error message.

## Example Use Cases

- **Text Recognition from Documents**: Upload images of scanned documents or printed text to extract their content.
- **Street Signs and Captions**: Extract text from photos of street signs, captions, or any image with visible text.
- **Quick Text Extraction**: Easily retrieve text from images of various formats without needing complex software setups.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
