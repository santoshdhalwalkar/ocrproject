# Custom OCR Project Using YOLOv3 and Tesseract

## Project Overview

#### This project aims to build a custom Optical Character Recognition (OCR) system by combining YOLOv3 for object detection and Tesseract for text extraction. It is designed to read specific contents of lab reports and convert them into an editable format. The implementation is done in Google Colab using Google Cloud OCR services for learning purposes.

## Objectives

#### 1. Detect specific text regions in lab reports using YOLOv3.

#### 2. Enhance image clarity through preprocessing techniques.

#### 3. Extract text from identified regions using Tesseract.

#### 4. Convert extracted data into an organized and editable CSV file.



## Tools & Technologies

Python: Core programming language

Google Colab: Development environment

YOLOv3: Object detection model

Tesseract OCR: Text recognition engine

OpenCV: Image processing library

Matplotlib: Visualization library

CSV Module: Data storage in CSV format



## Setup Instructions

Mount Google Drive:

Install Required Libraries:

!pip install opencv-python pytesseract
!sudo apt install tesseract-ocr libtesseract-dev


Download YOLOv3 Weights and Config Files:

!mkdir -p /content/drive/MyDrive/model
!wget -P /content/drive/MyDrive/model https://pjreddie.com/media/files/yolov3.weights
!wget -P /content/drive/MyDrive/model https://github.com/pjreddie/darknet/blob/master/cfg/yolov3.cfg?raw=true -O /content/drive/MyDrive/model/yolov3.cfg
!wget -P /content/drive/MyDrive/model https://github.com/pjreddie/darknet/blob/master/data/coco.names?raw=true -O /content/drive/MyDrive/model/coco.names


##Data Storage:

Store extracted text and image names in a CSV file
