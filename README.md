# Text-To-Sppech-conversion-using-OCR

Description:

This repository contains a Python script for Optical Character Recognition (OCR) using the Tesseract OCR engine and translation of the extracted text to a target language using the Google Translate API. 
The script supports both image and webcam input.


Getting Started

Prerequisites

Make sure you have the following installed:

1.Python

2.OpenCV (pip install opencv-python)

3.Tesseract OCR (pip install pytesseract)

4.Google Text-to-Speech (pip install gtts)

5.Playsound (pip install playsound)

6.Download and install the Tesseract OCR executable from Tesseract-OCR.

Setup
Clone the repository: git clone https://github.com/your-username/your-repo.git

Install the required packages: pip install -r requirements.txt

Set the path to your Tesseract OCR executable in the script:

pythonCopy code
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files (x86)\Tesseract-OCR\tesseract.exe"


Usage
Run the script:
python ocr_translation.py


1.The script will capture an image from the webcam and perform OCR on it.
2.The extracted text will be translated to a target language using the Google Translate API.
3.The translated text will be converted to speech and played.


Features
1.Image OCR: Extracts text from an input image (img2.jpg in the example).
2.Webcam OCR: Captures an image from the webcam and performs OCR on it.
3.Bounding Boxes: Displays bounding boxes around each character and word in the OCR output.
4.Translation: Translates the extracted text to a target language using the Google Translate API.
5.Text-to-Speech: Converts the translated text to speech and plays it.


Configuration:
Set the webcam properties (width and height) in the script:

cap.set(3, 640)  # Set width
cap.set(4, 480)  # Set height


Specify the Google Translate API key and endpoint in the script:

headers = {
    "content-type": "application/x-www-form-urlencoded",
    "X-RapidAPI-Key": "your-api-key",
    "X-RapidAPI-Host": "google-translate1.p.rapidapi.com"
}


Contributing
Fork the repository.
Create a new branch: git checkout -b feature/new-feature.
Commit your changes: git commit -am 'Add new feature'.
Push to the branch: git push origin feature/new-feature.
Submit a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.
