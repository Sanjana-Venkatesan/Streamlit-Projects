# Blog Outline Generator  

This **Blog Outline Generator** is a Streamlit web application that uses **Google's Gemini-Pro model** to generate comprehensive blog outlines based on a given topic. It also offers a **random topic suggestion** feature and interactive collapsible sections to improve readability.  

---

## Features 🛠️  

1. **Blog Outline Generation**  
   - Users can input any blog topic, and the app generates a detailed outline using Google's Gemini-Pro model.

2. **Random Topic Generator**  
   - Provides inspiration with randomly generated blog topics.

3. **Interactive Collapsible Sections**  
   - The generated blog outline is displayed with collapsible sections for improved readability.

4. **Custom Layout**  
   - Clean and responsive layout with two columns for user interaction and suggestions.  

---

## Technologies Used 💻  

- **Python**  
- **Streamlit**: To create the interactive web application.  
- **Google GenerativeAI API**: Integrates the **Gemini-Pro** model for content generation.  

---

## How It Works ⚙️  

1. **Input a Blog Topic**:  
   - Enter a topic in the text input field and click "Generate Outline" to get a structured blog outline.

2. **Random Topic Suggestion**:  
   - Use the **Generate Random Topic** button in the sidebar to get a random blog topic.  

3. **Collapsible Sections**:  
   - The generated outline is presented in collapsible sections to enhance readability and focus.

---

## Installation 🚀  

1. Clone the repository:  
   ```bash
   git clone <repo-url>
   cd blog-outline-generator
   ```  

2. Install dependencies:  
   ```bash
   pip install streamlit google-generativeai wordcloud  
   ```  

3. Run the Streamlit app:  
   ```bash
   streamlit run app.py  
   ```  

---

## Configuration ⚙️  

To use **Google's Gemini-Pro model**, replace the placeholder `api_key` in the script with your actual **Google API Key**:  
```python
genai.configure(api_key="YOUR_API_KEY_HERE")
```  

---

## Usage 🎯  

1. Open the app in your browser.  
2. Enter a blog topic and click **Generate Outline** to get the structured blog content.  
3. Explore collapsible sections for better navigation.  
4. Use the **Random Topic Generator** to get inspiration when needed.

---

## Example Output 📄  

### **Input**:  
**Topic**: Artificial Intelligence  

### **Output**:  
- Paragraph 1: *Introduction to AI and its applications.*  
- Paragraph 2: *Importance of AI in modern industries.*  
- Paragraph 3: *Future prospects and ethical considerations.*  

---

## Dependencies 📦  

- `streamlit`  
- `google-generativeai`  
- `wordcloud`  
- `random`  

---

## Author ✨  

**Sanjana Venkatesan**  
- [GitHub](https://github.com/Sanjana-Venkatesan)  
- [LinkedIn](#) *(Add your LinkedIn if applicable)*  

---

## License 📄  

This project is licensed under the **MIT License**.  
