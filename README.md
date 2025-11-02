📊 DataDigest – AI File Summarizer

[DataDigest is built to be your intelligent assistant that handles the “reading part”,so you can focus on the “thinking part.”]

How much time teams spend manually reading and interpreting long business reports, feedback files, and Excel summaries???

This made me realize how repetitive and inefficient this task really is.

Later, while discussing the concept with my professor, we talked about the growing role of AI in automating knowledge extraction, and how summarization models could bridge that exact gap.

And that’s how DataDigest came to life, An AI-powered tool that can read, understand, and summarize multi-format business documents in seconds.

This project combines my curiosity for Natural Language Processing (NLP) with practical, real-world problems faced by professionals every day.

🔷 Why I Built This

In most organizations, people spend hours every week reading raw Excel reports, lengthy Word documents, and unstructured feedback files,just to pull out key takeaways.

I wanted to build something that:

-Saves time by automating report analysis

-Extracts core insights from text-heavy documents

-Combines all summaries into a single, professional report

-Helps teams make decisions faster with less manual reading


🔷 Who Benefits from DataDigest

-Software Engineers & Data Analysts: Quickly extract insights from project reports, logs, and datasets.

-Corporate Teams & Managers : Get high-level overviews of operational or performance reports.

-Business Analysts – Instantly turn raw spreadsheets into meaningful summaries for decision-making.

-Researchers & Students – Summarize lengthy documents, papers, or lab data efficiently.


🔷 Folder Structure

📁DataDigest/
│
├── main.py                     # Streamlit main app file (core logic + UI)
├── setup_nltk.py               # Downloads required NLTK resources (punkt, stopwords)
│
├── venv/                       # Virtual environment (not pushed to GitHub)
│   ├── Lib/
│   ├── Scripts/
│   └── ... 
│
├── sample_files/               # Sample input files for testing (not pushed to github, stored locally for testing purpose)
│   ├── feedback.txt
│   ├── report1.docx
│   └── sales_report.xlsx
│
├── DataDigest_Summary_Report.pdf  # Auto-generated PDF summary output
│
├── .gitignore                  # Ignored files (like venv/, large files)
└── README.md                   # Project documentation


🔷 Features

-Multi-format File Support

-AI-Powered Summarization

-Automated PDF Report Generation

-Batch File Processing

🔷 Tech Stack

🔷 Frontend

-Streamlit

🔷 Backend

Python 3.10+

🔷 AI & NLP

-Hugging Face Transformers

-DistilBART-CNN-12-6

🔷 File Handling

-python-docx

-pandas

-UTF-8 Safe Reader

🔷 Report Generation

-FPDF

-Unicode Output

-Timestamped Reports

🔷 Version Control & Setup

-Git

-GitHub

-.gitignore

-venv

🔷 How It Works 

-Upload Files
You upload multiple files (.docx, .xlsx, .csv) via the Streamlit interface.

-File Reading & Text Extraction

.txt → decoded with UTF-8 for full compatibility

.docx → parsed paragraph by paragraph using python-docx

.xlsx / .csv → converted into a human-readable text format with pandas

-AI Summarization Engine
Extracted text is passed through the HuggingFace summarization pipeline, which compresses large documents into meaningful summaries (150–250 words).

-PDF Report Generation
All summaries are merged into one professional DataDigest Summary Report, formatted with file labels and generation timestamps.

-Instant Download
The final report is ready for download and review,clean, organized, and AI-written.

🔷 How to run it locally 

-Clone the Repository

git clone https://github.com/Shriya-23/DataDigest.git

cd DataDigest

-Create and Activate a Virtual Environment

For Windows:

python -m venv venv

venv\Scripts\activate

-Install All Dependencies

pip install streamlit transformers pandas python-docx openpyxl fpdf PyPDF2

-Run the Application

streamlit run main.py

💼 About Me

Hi! I’m Shriya Sharma, A Computer Science student passionate about building practical, data-driven, and impactful tech solutions.

I love transforming ideas into simple, meaningful tools that bridge the gap between technology and real-world problems.

💬 Got suggestions, feedback, or ideas?

 shriya.sharma1923@gmail.com
