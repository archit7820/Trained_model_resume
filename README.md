# Resume Verse


A FastAPI-based application for parsing resumes, analyzing job descriptions, and generating interview questions. This project simplifies the resume screening process by automating key tasks like scoring resumes and aligning them with job descriptions.

## Features

- Upload resumes in `PDF`, `DOCX`, or `TXT` formats.
- Parse and extract key information from resumes and job descriptions.
- Summarize resume content.
- Score resumes based on job descriptions.
- Generate interview questions when alignment is sufficient.
- Provides an interactive HTML interface for file upload.

## Installation

### Prerequisites

- Python 3.8 or higher
- Virtual environment setup (recommended)

### Steps

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd resume_verse
   ```


   Set up a virtual environment:
   
###  start 
    ```bash
            python -m venv venv
            .\venv\Scripts\activate  
            python -m uvicorn main:app --reload
            pip install -r requirements.txt
    ```

    Access the app in your browser at:
        http://127.0.0.1:8000


###  structure 

        <svg version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 869.7590942382812 320.00000000000006" width="869.7590942382812" height="320.00000000000006"><!-- svg-source:excalidraw --><metadata></metadata><defs><style class="style-fonts">
      @font-face { font-family: Excalifont; src: url(data:font/woff2;base64,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); }</style></defs><rect x="0" y="0" width="869.7590942382812" height="320.00000000000006" fill="#ffffff"></rect><g transform="translate(10 10) rotate(0 424.8795471191406 150.00000000000003)"><text x="0" y="17.619999999999997" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">resume_verse/</text><text x="0" y="42.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">│</text><text x="0" y="67.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">├── app/</text><text x="0" y="92.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">│   ├── models/           # Logic for parsing and scoring resumes and job descriptions</text><text x="0" y="117.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">│   ├── templates/        # HTML templates for the application</text><text x="0" y="142.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">│   ├── main.py           # FastAPI application entry point</text><text x="0" y="167.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">│</text><text x="0" y="192.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">├── uploads/              # Directory to store uploaded files</text><text x="0" y="217.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">├── README.md             # Project documentation</text><text x="0" y="242.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">├── requirements.txt      # Python dependencies</text><text x="0" y="267.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic">└── venv/                 # Virtual environment (optional)</text><text x="0" y="292.62" font-family="Excalifont, Xiaolai, Segoe UI Emoji" font-size="20px" fill="#1e1e1e" text-anchor="start" style="white-space: pre;" direction="ltr" dominant-baseline="alphabetic"></text></g></svg>



    API Endpoints
    GET /
    Renders the HTML upload form.


    POST /upload
    Uploads and processes a resume and job description.
    Request: Multipart form data with file and job_description.
    Response:
    json
    {
        "summary": "Summarized content of the resume",
        "score": 85,
        "alignment": 90,
        "questions": ["What is your experience with Python?", "Explain your leadership roles."]
    }

    Technologies Used
    FastAPI: Backend framework
    Jinja2: Template rendering
    PyPDF2: PDF parsing
    python-docx: Word document parsing


    Contributing
    Fork the repository.
    Create a new branch (git checkout -b feature-name).
    Commit your changes (git commit -m 'Add feature').
    Push to the branch (git push origin feature-name).
    Create a pull request.