# Image-Based Book Recommendation 📚  

This **Image-Based Book Recommendation** app leverages **Google's Gemini Pro Vision API** to analyze an uploaded image and provide relevant book recommendations based on its content.  

---

## Features 🛠️  

1. **Image Input Options**:  
   - Upload an image directly.  
   - Provide an image URL for analysis.  

2. **Book Recommendation**:  
   - Uses **Gemini Pro Vision** to understand the image content.  
   - Provides a book recommendation along with a short explanation (5 words) of its relevance to the image.  

3. **Image Display**:  
   - Resizes and displays the uploaded or fetched image for clarity.  

---

## Technologies Used 💻  

- **Streamlit**: For creating the web interface.  
- **Pillow (PIL)**: For image processing.  
- **Google Gemini Pro Vision**: For analyzing the image and generating recommendations.  
- **Requests**: For fetching image data from a URL.  

---

## How It Works ⚙️  

1. **Input Image**:  
   - Users can upload an image file (JPG, PNG) or provide a URL.  

2. **Gemini Vision API**:  
   - The app processes the image and queries the **Gemini Pro Vision model** for a book recommendation.  

3. **Output**:  
   - Displays the image and provides a book recommendation with a brief explanation.  

---

## Installation 🚀  

1. Clone the repository:  
   ```bash
   git clone <repo-url>
   cd image-book-recommendation
   ```

2. Install dependencies:  
   ```bash
   pip install streamlit pillow requests langchain langchain-google-genai  
   ```

3. Run the Streamlit app:  
   ```bash
   streamlit run app.py  
   ```

---

## Usage 🎯  

1. Open the app in your browser (e.g., `http://localhost:8501`).  
2. **Choose Input Option**:  
   - Upload an image or provide an image URL.  
3. **Generate Recommendation**:  
   - Once processed, the app displays the uploaded image and a relevant book recommendation.  

---

## Example Output 📄  

### **Input**:  
- **Image**: An image related to nature or technology.  

### **Output**:  
- **Book Recommendation**: "The Overstory" by Richard Powers.  
- **Reason**: "Nature’s beauty inspires human connection."  

---

## API Configuration 🔑  

- Replace the `google_api_key` in the code with your **Google API Key** to use Gemini Pro Vision.  

---

## Dependencies 📦  

- `streamlit`  
- `Pillow`  
- `requests`  
- `langchain`  
- `langchain-google-genai`  

---

## Limitations ⚠️  

- Ensure your Google API key has access to **Gemini Pro Vision**.  
- Input images should be clear and relevant to produce accurate recommendations.  

---

## Author ✨  

**Sanjana Venkatesan**  
- [GitHub](https://github.com/Sanjana-Venkatesan)  
- [LinkedIn](#)

---

## License 📄  

This project is licensed under the **MIT License**.  
