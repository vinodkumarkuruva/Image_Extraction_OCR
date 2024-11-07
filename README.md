## Title : 
OCR Text Extractor

## Description : 
This project is a simple Optical Character Recognition (OCR) tool that extracts text from images using Python's Tesseract OCR library. Given an image path, the tool uses pre-processing techniques to enhance text readability and then extracts text using Tesseract OCR.

## Features

- Resizes images for improved accuracy
- Converts images to grayscale for enhanced contrast
- Uses "pytesseract" for text extraction

 ## Prerequisites

Ensure you have the following installed:

- **Python 3.x**
- **Tesseract OCR**: Download and install Tesseract from [Tesseract OCR](https://github.com/tesseract-ocr/tesseract). Ensure the installation path is correct and updated in the code.

## Installation

1. Clone this repository:
     git clone https://github.com/vinodkumarkuruva/Image_Extraction_OCR.git
     cd ocr-text-extractor

2. Installation :

   pip install -r requirements.txt

3. Update the tesseract_cmd path in the script to point to your local installation of Tesseract:

     pytesseract.pytesseract.tesseract_cmd = r'c:\Program Files\Tesseract-OCR\tesseract.exe'

## Configuration

- Tesseract executable path: If your system does not automatically detect the Tesseract executable, you will need to set the pytesseract.pytesseract.tesseract_cmd variable in the script(Line 7) to the correct path.

    python ocr_text_extractor.py path/to/your/imagefile.jpg

## Future explorations

- Create a User Interface (UI) to edit processed Text, allowing additional features like text selection, formatting options, and the ability to correct any OCR errors. This also allows users to copy the extracted text and paste it directly into other applications or forms. This will make it easier to use the extracted text for various purposes, such as data entry or content generation.

- Implement a for loop that processes each image one by one and outputs the extracted text for all images in a single run. This will streamline the text extraction process for large volumes of images.

- Continue experimenting with different image pre-processing techniques to further improve OCR accuracy.

- Optimize performance by using multi-threading or multiprocessing to help speed up the text extraction process.

- Integrate natural language processing techniques to perform advanced analysis such as keyword extraction on the extracted text.

