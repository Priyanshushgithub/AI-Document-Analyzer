## 📄 Overview
AI Document Analyzer and Keyword Extractor is a Python-based web application that automates document analysis using Optical Character Recognition (OCR) and Natural Language Processing (NLP).

The application allows users to upload documents in multiple formats such as PDF, images, and text files. It extracts textual content from these documents and leverages IBM Watson Natural Language Understanding (NLU) to identify important keywords and named entities.

This project demonstrates the integration of OCR technologies, cloud-based NLP services, and web application development to create an intelligent document-processing solution.

This project is developed for educational and research purposes as part of an academic cloud computing and AI initiative.

---

## 🚀 Features
- Upload documents in multiple formats:
  - PDF (.pdf)
  - Text (.txt)
  - Images (.jpg, .jpeg, .png)
- Optical Character Recognition (OCR) using Tesseract
- PDF text extraction using PyMuPDF
- Keyword extraction using IBM Watson NLU
- Named Entity Recognition (People, Organizations, Locations, etc.)
- View extracted text on the web interface
- Download analysis report
- User-friendly Flask web application

---

  
  ## 🛠 Technologies Used

| Technology          | Purpose                     |
|---------------------|-----------------------------|
| Python              | Programming Language        |
| Flask               | Web Framework               |
| HTML/CSS/JavaScript | Frontend                    |
| Tesseract OCR       | Image Text Extraction       |
| PyMuPDF (fitz)      | PDF Text Extraction         |
| IBM Watson NLU      | Keyword & Entity Extraction |
| Pillow              | Image Processing            |
| IBM Cloud           | Cloud-based AI Services     |

## 🏗 Project Architecture

```
                 User
                  │
                  ▼
        HTML/CSS/JavaScript
                  │
                  ▼
            Flask Backend
                  │
        ┌─────────┴─────────┐
        ▼                   ▼
  Text Extraction      IBM Watson NLU
 (OCR / PDF / TXT)     Keyword Analysis
        │                   │
        └─────────┬─────────┘
                  ▼
          Analysis Results
                  │
                  ▼
          Download Report
```

---

## ⚙ Workflow

### Step 1
Upload a document (PDF, Image, or Text file).

### Step 2
Extract text using:
- Tesseract OCR for Images
- PyMuPDF for PDFs
- Direct reading for Text files

### Step 3
Send extracted text to IBM Watson Natural Language Understanding.

### Step 4
Analyze the text to extract:
- Keywords
- Named Entities

### Step 5
Display results on the web application.

### Step 6
Download the generated report.

---

## 📂 Supported File Formats

- PDF (.pdf)
- JPG (.jpg)
- JPEG (.jpeg)
- PNG (.png)
- TXT (.txt)

---

## 📁 Project Structure

```
AI-Document-Analyzer/
│
├── app.py
├── templates/
│   └── index.html
├── static/
│   └── result.txt
├── uploads/
├── requirements.txt
└── README.md
```

---

## 🔧 Installation

### Clone Repository

```bash
git clone https://github.com/your-username/AI-Document-Analyzer.git
cd AI-Document-Analyzer
```

### Install Dependencies

```bash
pip install flask
pip install pytesseract
pip install pillow
pip install pymupdf
pip install ibm-watson
```

Or install everything using:

```bash
pip install -r requirements.txt
```

---

## Install Tesseract OCR

### Windows

Download from:

https://github.com/tesseract-ocr/tesseract

Configure its path inside `app.py`:

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

### Linux

```bash
sudo apt install tesseract-ocr
```

---

## IBM Cloud Configuration

Create an IBM Cloud account and provision an IBM Watson Natural Language Understanding service.

Add your credentials:

```python
API_KEY = "YOUR_API_KEY"
SERVICE_URL = "YOUR_SERVICE_URL"
```

---

## ▶ Running the Application

```bash
python app.py
```

Open your browser:

```
http://127.0.0.1:5000
```

---

## 📊 Sample Output

### Extracted Keywords

- Artificial Intelligence
- Machine Learning
- Cloud Computing
- Data Analytics

### Detected Entities

- IBM
- Google
- Bengaluru
- Python

---

## 💡 Applications

- Resume Analysis
- Research Paper Analysis
- Invoice Processing
- Medical Document Analysis
- Legal Document Analysis
- Enterprise Document Management
- OCR-based Digitization

---

## 🔮 Future Enhancements

- IBM Cloud Object Storage Integration
- AI-based Document Classification
- Sentiment Analysis
- Emotion Detection
- Multi-language OCR Support
- User Authentication
- Dashboard Analytics
- Document History Management

---

## 👨‍💻 Contributors

- Priyanshu Sharma
- Satish Mallappa B Patil
- Kishor C
- Albin Akkara

---
