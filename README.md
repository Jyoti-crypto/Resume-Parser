# Resume-Parser
Resume Parser-Developed an ai system to extract and organize information from resumes enhancing,HR processes and candidate selection
# Resume Parser AI (PDF Resume Extractor)

This project is a **Resume Parser** that extracts key details such as Name, Contact Number, Email, Skills, and Education from resumes in **PDF format** using Natural Language Processing (NLP).

---

## 🚀 Features

- Extracts:
  - Full Name (using spaCy NER)
  - Contact Number (Regex)
  - Email ID (Regex)
  - Key Skills (Pattern Matching)
  - Education Qualifications (Regex + Keyword Search)
- Supports PDF upload in Google Colab
- Graceful fallback to "NA" for missing data

---

## 🛠️ How to Run the Code

### ▶️ On Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload the `Resume_Parser.ipynb` notebook.
3. Run each cell sequentially.
4. It will prompt you to upload a **PDF resume**.
5. The extracted details will be printed as output.

> Ensure your resume is a **text-based PDF** (not scanned image).

---

## 📁 Folder Structur
Resume_Parser/
│
├── Resume_Parser.ipynb # Main Jupyter Notebook
├── README.md # This file
└── sample_resume.pdf # (Optional) Sample resume for testing

---

## 🔧 Technologies Used

- **Python**
- **Google Colab**
- **spaCy** – For Name Entity Recognition (NER)
- **pdfminer.six** – For text extraction from PDF
- **Regex** – For pattern-based extraction

---

## 📚 Core Methodologies

| Feature     | Methodology                                     |
|-------------|--------------------------------------------------|
| Name        | Named Entity Recognition with `spaCy`           |
| Contact     | Regular Expressions for phone number patterns    |
| Email       | Regex pattern for email detection                |
| Skills      | Keyword-based matching from a skill list         |
| Education   | Regex patterns for common degrees (B.Tech, MBA)  |

---


## ✅ Sample Output
Name: John Doe
Contact Number: +1 987-654-3210
Email: john.doe@example.com
Skills: ['Python', 'SQL', 'Machine Learning']
Education: ['B.Tech in Computer Science']


