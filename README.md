﻿# AI_Resume_Parser
 Here's a basic README file for an AI Resume Parser project:

---

# AI Resume Parser

## Overview
The AI Resume Parser is a tool designed to automatically extract relevant information from resumes in various formats (PDF, DOCX, etc.) and convert it into structured data. This data can be easily used for further analysis or integration into recruitment systems, making the hiring process faster and more efficient.

## Features
- Automatic Data Extraction: Extracts key information like name, contact details, work experience, education, skills, and more.
- Multi-Format Support: Processes resumes in formats such as PDF, DOCX, TXT, etc.
- Configurable Output: Structured data in JSON or CSV formats for easy integration.
- Keyword Matching: Identifies specific keywords related to job descriptions for better candidate fit analysis.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Kaushikj14/AI_Resume_Parser.git
   cd AI_Resume_Parser.git
   ```

2. **Set up a virtual environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # For MacOS/Linux
   venv\Scripts\activate      # For Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download NLP models (if applicable):**
   Download language models required for natural language processing (NLP). Example with SpaCy:
   ```bash
   python -m spacy download en_core_web_sm
   ```

## Usage

1. **Place the resume files in the `resumes` folder.**
2. **Run the parser script:**
   ```bash
   python app.py
   ```
3. **Output**: The parsed information will be saved as a structured JSON or CSV file in the `output` directory.

## Example Output

The output data is organized in a structured format (JSON or CSV) with the following fields:

```json
{
  "name": "John Doe",
  "contact": {
    "email": "john.doe@example.com",
    "phone": "+123456789"
  },
  "education": [
    {
      "degree": "B.Sc. in Computer Science",
      "institution": "University of XYZ",
      "year": "2020"
    }
  ],
  "experience": [
    {
      "job_title": "Software Engineer",
      "company": "TechCorp Inc.",
      "duration": "2021 - Present",
      "description": "Developing and optimizing software solutions."
    }
  ],
  "skills": ["Python", "Machine Learning", "Data Analysis"]
}
```

## Technologies Used
- Python: Core programming language
- Pandas: Data manipulation and export
- Regular Expressions: Pattern matching for text extraction
- Machine Learning Models: For keyword and entity recognition
- Generative ai : For using gen ai

## Contributing
Contributions are welcome! Please open an issue or submit a pull request if you'd like to contribute to this project.

## License
This project is licensed under the MIT License. See `LICENSE` for details.

---

This README provides a basic overview of the project, instructions for installation, usage, and a sample output, which will help new users get started with the AI Resume Parser project. Let me know if you'd like to add any other sections or details!
