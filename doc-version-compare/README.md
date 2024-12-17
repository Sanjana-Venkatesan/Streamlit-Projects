# Document Comparison

This Streamlit application allows users to upload and compare two PDF documents to highlight the differences between them. It reads the content of the PDF files, compares them line by line, and displays the differences in a user-friendly format.

## Features

- **Document Upload**: Allows users to upload two PDF documents.
- **Content Comparison**: The application compares the content of the two documents line by line and identifies differences.
- **User-Friendly Display**: The differences are displayed in a clear and readable format, with new lines added in the second document highlighted.
- **No Difference Handling**: If no differences are found, the app notifies the user accordingly.
  
## Requirements

Ensure you have the following Python libraries installed:

- **Streamlit**: For creating the web app interface.
- **difflib**: For comparing the text content of the documents.
- **textwrap**: For formatting the text to ensure it fits within the display width.
- **PyPDF2** (or any other PDF library): If needed, use it for extracting text from PDFs. (Although it's not explicitly included in the provided code, if necessary, you can install it for more advanced PDF handling).

To install the required libraries, use the following:

```bash
pip install streamlit
```

## Setup

1. **Install Streamlit**: If you haven’t already installed Streamlit, run the following command:
    ```bash
    pip install streamlit
    ```

2. **Run the App**: After setting up the necessary libraries, save the script as `document_comparison.py` (or any name you prefer), and run the app using the following command:

    ```bash
    streamlit run document_comparison.py
    ```

    This will open the app in your default web browser.

## How It Works

1. **Upload Two PDFs**:
    - Users upload two PDF documents via the file uploader interface.
   
2. **Document Comparison**:
    - Upon clicking the "Compare Documents" button, the content of the two PDFs is read and compared line by line.
    - The app will display the differences, focusing on the new lines added in the second version of the document.

3. **Displaying the Differences**:
    - The differences are shown in a clean and readable format. The text is wrapped to ensure that it fits within the display width.

4. **No Differences**:
    - If no differences are found between the two documents, the app will notify the user that the documents are identical.

## File Structure

- **document_comparison.py**: The main Python script that runs the Streamlit app.
- **Requirements**: A `requirements.txt` file can be added for easy installation of dependencies (optional).

## Additional Notes

- **PDF Text Extraction**: The code currently assumes that the PDF content can be extracted as plain text. You can use libraries like `PyPDF2` or `pdfminer` for more robust text extraction from PDF files if needed.
  
- **Text Formatting**: The text in the comparison results is wrapped at 70 characters to ensure it fits within the Streamlit display width. This can be adjusted based on the layout requirements.

- **Limitations**:
  - The current implementation compares the raw text of the PDFs. It does not consider advanced document formatting (such as images, tables, or other non-text content).
  - Text extraction from PDFs can vary in quality depending on the PDF format (e.g., scanned PDFs vs. text-based PDFs).

## License

This project is open-source and can be used and modified freely for personal or educational purposes. For commercial use, please ensure compliance with the necessary licenses of third-party libraries used.
