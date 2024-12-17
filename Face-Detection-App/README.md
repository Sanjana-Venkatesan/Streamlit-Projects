# Face Detection App  

This **Face Detection App** is a Streamlit web application that detects faces in an image using OpenCV's Haar Cascade Classifier. Users can upload an image via a URL, and the app highlights detected faces with bounding boxes.

---

## Features 🛠️  

1. **Image Upload via URL**:  
   - Users can input the URL of an image to upload it into the app.

2. **Face Detection**:  
   - Uses OpenCV's Haar Cascade Classifier to detect faces in the provided image.

3. **Visual Results**:  
   - Displays both the original image and the processed image with detected faces.

4. **User-Friendly Interface**:  
   - Built with Streamlit for clean, interactive, and responsive UI.

---

## Technologies Used 💻  

- **Streamlit**: For creating the web interface.  
- **OpenCV (cv2)**: For image processing and face detection.  
- **Matplotlib**: For optional visualization.  
- **Requests**: For fetching images via URL.  
- **NumPy**: For handling image arrays.  

---

## How It Works ⚙️  

1. **Enter Image URL**:  
   - The user provides the URL of an image containing faces.

2. **Face Detection**:  
   - When the **Detect Faces** button is clicked, the app processes the image using OpenCV's Haar Cascade Classifier.

3. **Result Display**:  
   - The app displays the original image and the face-detected image with bounding boxes around detected faces.

---

## Installation 🚀  

1. Clone the repository:  
   ```bash
   git clone <repo-url>
   cd face-detection-app
   ```

2. Install dependencies:  
   ```bash
   pip install streamlit opencv-python-headless matplotlib requests numpy  
   ```

3. Run the Streamlit app:  
   ```bash
   streamlit run app.py  
   ```

---

## Usage 🎯  

1. Open the app in your browser (e.g., `http://localhost:8501`).  
2. Enter the URL of the image containing faces.  
3. Click the **"Detect Faces"** button to view results.  

---

## Example Output 📄  

### **Input**:  
- **Image URL**: URL of an image with human faces.

### **Output**:  
- Original Image: Displayed as uploaded.  
- Detected Faces: Bounding boxes drawn around faces.  

---

## Dependencies 📦  

- `streamlit`  
- `opencv-python-headless`  
- `requests`  
- `numpy`  
- `matplotlib`  

---

## Limitations ⚠️  

- This app uses Haar Cascade Classifier, which works well for frontal faces but may not detect faces in tilted or low-quality images.  
- Ensure the provided image URL is accessible and points to a valid image file.  

---

## Author ✨  

**Sanjana Venkatesan**  
- [GitHub](https://github.com/Sanjana-Venkatesan)  
- [LinkedIn](#) *(Optional: Add your LinkedIn profile link)*  

---

## License 📄  

This project is licensed under the **MIT License**.  
