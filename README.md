# Resume-PRO

The Resume-Screening project leverages a Large Language Model (LLM) to automate the process of evaluating resumes against job descriptions. The system analyzes resumes in PDF format, extracts relevant content using OCR (Optical Character Recognition), and compares it with the job description provided by the user.

## Features

- **Resume Evaluation**: Automatically evaluates resumes against job descriptions to assess how well the resume aligns with the job requirements.
- **OCR Integration**: Extracts relevant content from resumes in PDF format using Optical Character Recognition (OCR).
- **Job Description Analysis**: Compares the provided job description with the extracted resume content to evaluate the quality, relevance, and ATS compatibility.

## Sections

### 1. Title: "Resume Evaluation"
   - **Purpose**: Clearly indicates the functionality of the platform, which is to evaluate resumes against job descriptions.

### 2. Job Description Field
   - **Label**: "Job Description: Paste the job description here…"
   - **Description**: This field allows users to paste the text of a job description.
   - **Functionality**: By inputting a job description, the platform evaluates how well the resume aligns with the job requirements.

### 3. Prompt Type Dropdown
   - **Label**: "Prompt Type:"
   - **Options**:
     - **Evaluation**:
       - Focuses on assessing the overall quality, structure, and effectiveness of the resume.
       - Includes feedback on formatting, content relevancy, and skills alignment with the job description.
     - **ATS (Applicant Tracking System)**:
       - Checks the resume's compatibility with ATS software.
       - Ensures proper formatting, keyword density, and absence of ATS-blocking elements (such as images or complex designs).
   - **Default Selection**: Evaluation is selected by default in the dropdown.

### 4. Resume Upload Section
   - **Label**: "Upload Resume (PDF):"
   - **Functionality**: Provides an option for users to upload their resume in PDF format for evaluation.
   - **File Restrictions**: Accepts only PDF files to ensure compatibility with the OCR processing.

### 5. Submit Button
   - **Purpose**: Once the user pastes the job description, selects the evaluation type, and uploads the resume, clicking this button initiates the evaluation process.
## Technologies Used

- **Django**: Web framework for building the application.
- **Python**: Primary language for backend logic.
- **OCR (Optical Character Recognition)**: Used to extract text from resumes in PDF format.
- **Large Language Model (LLM)**: `llama-3.2-90b-vision-preview` for analyzing and evaluating resumes against job descriptions.
