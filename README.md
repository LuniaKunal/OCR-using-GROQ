# OCR Using GROQ

## Overview
This project is a mini Optical Character Recognition (OCR) system developed using **GROQ**. OCR systems are used to extract and digitize text from images or scanned documents. By leveraging the capabilities of GROQ, this project achieves efficient and accurate text recognition.

---

## Features
- **Image Preprocessing**: Optimizes the input image for OCR by resizing, noise removal, and binarization.
- **Text Detection**: Identifies and extracts text regions from images.
- **Text Recognition**: Converts the detected text regions into readable text.
- **Integration with GROQ**: Utilizes GROQ’s processing capabilities for enhanced performance and accuracy.

---

## Prerequisites
To run this project, you need the following:
- Python 3.8 or later
- GROQ SDK installed on your machine
- Required Python libraries:
  - OpenCV
  - NumPy
  - PIL (Pillow)
  - pytesseract

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ocr-mini-project-groq.git
   cd ocr-mini-project-groq
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure GROQ SDK is installed and configured on your system.
4. Install Tesseract OCR (if not already installed):
   ```bash
   # For Ubuntu
   sudo apt update
   sudo apt install tesseract-ocr

   # For Windows or macOS
   # Follow instructions at https://github.com/tesseract-ocr/tesseract
   ```

---

## Usage
1. Place the image(s) to be processed in the `input_images` folder.
2. Run the script:
   ```bash
   python ocr_groq.py
   ```
3. View the extracted text in the terminal or in the `output_text` folder.

---

## File Structure
```
.
├── input_images/        # Folder for input images
├── output_text/         # Folder for extracted text files
├── ocr_groq.py          # Main script for the OCR system
├── requirements.txt     # List of Python dependencies
├── README.md            # Project documentation
```

---

## How It Works
1. **Preprocessing**: The input image is processed to enhance text readability by adjusting brightness, removing noise, and binarizing the image.
2. **Text Detection**: GROQ accelerates the detection of text regions in the image.
3. **Text Recognition**: The detected regions are processed using Tesseract OCR to extract the text.
4. **Output**: The extracted text is saved in the `output_text` folder.

---

## Example
Input image:
![Input Image](./examples/sample_input.jpg)

Extracted text:
```
Hello World!
This is an OCR example powered by GROQ.
```

---

## Future Enhancements
- Add support for multi-language OCR.
- Improve text detection using deep learning models.
- Incorporate real-time OCR capabilities for video feeds.
- Implement a web-based interface for easier usage.

---

## Contributing
Contributions are welcome! Please create a pull request or open an issue if you have suggestions or improvements.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments
- [GROQ](https://groq.com) for providing the processing framework.
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) for text recognition.
- OpenCV and PIL for image processing functionalities.
