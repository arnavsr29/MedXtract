## SCT_DS_2

# MedXtract - A Medical Data Extraction Project
This project focused on developing an Optical Character Recognition (OCR) system to extract critical information from PDF documents, specifically targeting patient and prescription details. The system was designed to automate the process of retrieving and organizing relevant medical data from potentially complex and varied document formats. Additionally, the project involved the creation of a robust backend server that handled incoming data extraction requests. This server acted as the processing hub, efficiently managing and executing OCR tasks, ensuring seamless integration and real-time data extraction for the user interface or external applications.

## Project Overview
## 1. What is OCR?
OCR (Optical Character Recognition) Converts scanned documents, PDFs, and images into machine-readable text.</br>
Uses machine learning, including CNNs, to enhance text recognition, accuracy, and context comprehension, continuously learning and adapting to new domains and languages.

![2](https://github.com/user-attachments/assets/d740107c-4e3c-4b77-ba92-c97d84d866d8)
</br>

## 2. Introduction to Project $ Demo using Visualization.
For this project we have two types of Medical Documents.
1. Patient Medical Record
2. Prescription

We are going to extract some important fields from these documents.

![3](https://github.com/user-attachments/assets/432645a3-05d4-42a3-8f8a-ef67eae8d620)
![4](https://github.com/user-attachments/assets/1ba131c3-7f5b-41b3-839f-3337874e917d)

</br>

## 3. Project Execution Steps
- Step 1: Convert pdf to image using `pdf2image` library
- Step 2: Preprocess the image (Apply `adaptive thresholding and binarization using OpenCV2`)
- Step 3: Extracting text from image by passing it through `tesseract OCR engine`
- Step 4: Finding useful information from text using `RegEx` and returning in JSON format
- Step 5: Creating a `FastAPI backend server` which serves data extraction requests by accepting a pdf_file, file_format and returning a JSON object.
- Step 6: To create a Demo of `frontend UI using Streamlit` and connect it with our FastAPI server using Python Requests module.
- 
![5](https://github.com/user-attachments/assets/b45ca52d-4d01-4301-8df5-f9ef99f74fc0)
</br>

## 4. Code Walkthrough
- Notebook 1: [Prescription_parser]
- Notebook 2: [Patient_details_parser]
- Backend: [Source code directory]
- Frontend: [Streamlit app]
- 
![6](https://github.com/user-attachments/assets/4d4ee83f-4d81-4d47-9c6a-280a9a3ac17c)
</br>

## 5. What did I learn through this project?
- Applied OCR in real-world projects by leveraging key image processing techniques, such as thresholding, using the OpenCV2 library.
- Sharpened Python coding with OOP, code refactoring, and modular programming.
- Set up a backend server using the FastAPI framework.
- Connected a Streamlit frontend to a FastAPI backend using the requests module in Python.
