## SCT_DS_2

# MedXtract - A Medical Data Extraction Project
This project focused on developing an Optical Character Recognition (OCR) system to extract critical information from PDF documents, specifically targeting patient and prescription details. The system was designed to automate the process of retrieving and organizing relevant medical data from potentially complex and varied document formats. Additionally, the project involved the creation of a robust backend server that handled incoming data extraction requests. This server acted as the processing hub, efficiently managing and executing OCR tasks, ensuring seamless integration and real-time data extraction for the user interface or external applications.

## Project Overview
## 1. What is OCR?
OCR (Optical Character Recognition) Converts scanned documents, PDFs, and images into machine-readable text.</br>
Uses machine learning, including CNNs, to enhance text recognition, accuracy, and context comprehension, continuously learning and adapting to new domains and languages.

![2](https://github.com/user-attachments/assets/a0462f3c-d208-4817-a451-49fd8eef7976)

</br>

## 2. Introduction to Project $ Demo using Visualization.
For this project we have two types of Medical Documents.
1. Patient Medical Record
2. Prescription

We are going to extract some important fields from these documents.

![3](https://github.com/user-attachments/assets/e245ca95-1b66-44be-98ae-3c2d4825cc5e)
![4](https://github.com/user-attachments/assets/51c874af-11db-41c7-8bc9-cc42d298ca24)

</br>

## 3. Project Execution Steps
- Step 1: Convert pdf to image using `pdf2image` library
- Step 2: Preprocess the image (Apply `adaptive thresholding and binarization using OpenCV2`)
- Step 3: Extracting text from image by passing it through `tesseract OCR engine`
- Step 4: Finding useful information from text using `RegEx` and returning in JSON format
- Step 5: Creating a `FastAPI backend server` which serves data extraction requests by accepting a pdf_file, file_format and returning a JSON object.
- Step 6: To create a Demo of `frontend UI using Streamlit` and connect it with our FastAPI server using Python Requests module.

![5](https://github.com/user-attachments/assets/7d84ea38-919e-4d38-b708-69437594785c)

</br>

## 4. Code Walkthrough
- Notebook 1: [Prescription_parser]
- Notebook 2: [Patient_details_parser]
- Backend: [Source code directory]
- Frontend: [Streamlit app]

![6](https://github.com/user-attachments/assets/49b45913-cefc-4d4e-b46a-2ba977d332c7)

</br>

## 5. What did I learn through this project?
- Applied OCR in real-world projects by leveraging key image processing techniques, such as thresholding, using the OpenCV2 library.
- Sharpened Python coding with OOP, code refactoring, and modular programming.
- Set up a backend server using the FastAPI framework.
- Connected a Streamlit frontend to a FastAPI backend using the requests module in Python.
