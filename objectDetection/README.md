# Object Detection App with Streamlit 📸🔍

This is an **Object Detection app** built with **Streamlit** and **PyTorch** using the **Faster R-CNN model** to detect and label objects in images. Users can either upload an image or provide an image URL for object detection. The app visualizes the image with bounding boxes around detected objects and displays prediction details.

## Features

- **Upload Image**: Users can upload an image for object detection.
- **Provide Image URL**: Users can provide an image URL for detection.
- **Bounding Boxes**: Detected objects are highlighted with bounding boxes, with colors representing different object categories.
- **Predictions**: The app displays predicted labels and their corresponding probabilities for each detected object.

## Prerequisites

Before running the application, ensure that you have the following dependencies:

- Python 3.x
- Streamlit
- PyTorch
- PIL (Pillow)
- Matplotlib
- Requests

### Install the required dependencies

```bash
pip install streamlit torch torchvision pillow matplotlib requests
```

## Setup

1. **Clone or create the app**: Copy the script into your local directory.
2. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

3. Open your browser and go to `http://localhost:8501` to use the app.

## How It Works

1. **Choose Input Option**: You can either upload an image or provide an image URL for object detection.
2. **Object Detection**: The app processes the image using the pre-trained **Faster R-CNN** model, detects objects, and draws bounding boxes around the identified objects.
3. **Prediction Display**: The app shows the predicted labels and their respective probabilities for each detected object.

### Model Used

The model used for object detection is **Faster R-CNN** with a **ResNet50-FPN backbone**, pre-trained on the COCO dataset. The app uses this model to detect objects in uploaded or provided images.

### Key Points:

- **Bounding Box Colors**: Objects identified as "person" are marked with **red** bounding boxes, while other objects have **green** bounding boxes.
- **Predicted Labels and Probabilities**: After the bounding boxes are drawn, the app displays the detected labels and their prediction scores.

## How to Use

1. **Upload Image**: Select "Upload Image" from the options, and then upload a local image file (PNG, JPG, JPEG).
2. **Provide Image URL**: Select "Provide Image URL" and enter the URL of an image from the web.

The app will automatically detect objects in the image and display them with bounding boxes.

## Customization

You can customize or expand the app to include:
- **Additional models**: Replace the Faster R-CNN model with other models for object detection if needed.
- **Detection Threshold**: Adjust the detection threshold for better or more precise predictions.
- **UI Enhancements**: Modify the Streamlit interface for a better user experience or add more options (e.g., adjust bounding box colors, select detection categories, etc.).

## License

This project is licensed under the **MIT License**.

