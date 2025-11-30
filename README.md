# Smart-Career-Application Assistant (SCAA)


# Google × Kaggle Agents Intensive – Capstone Project
# 🏆 Hackathon Writeup
A simple and intelligent AI-powered career assistant that helps job seekers analyze their resume, extract skills, get job role recommendations, check market trends, and generate professional cover letters — all inside a single Kaggle Notebook.
![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/SCAA.png?raw=true)

# Team Members
Priyanka

Monika Dhukia

Shrishti Yadav

# 🚀 Project Overview
The Smart Career Application Assistant (SCAA) uses Google’s Agent Development Kit (ADK) and Gemini LLM to understand resumes and give helpful career guidance.
The system automatically:

📄 Reads and extracts text from a PDF resume

🎯 Identifies technical & soft skills (custom Python skill extractor)

💼 Suggests job roles matching the user profile

📊 Retrieves real-time job market trends using Google Search

✍️ Generates a short, personalized cover letter

🧩 Provides resume improvement suggestions

 ✍️ This makes the job preparation process much faster and easier.
 
⭐ This turns hours of manual research into a 60-second automated process.

# Problem Statement
- Job seekers often struggle with:

- Understanding what their resume communicates

- Identifying their strongest skills

- Matching themselves to the right job roles

- Researching market trends, salaries, and in-demand skills

- Writing a clean, professional cover letter

- The process is slow, confusing, and often leads to missed opportunities.

# ⭐ SCAA Solve this:
⚡ Saves Time
Instantly analyzes a resume and provides structured insights.

🎯 Accurate Skill Extraction
Custom Python extractor identifies relevant technical & soft skills.

💼 Personalized Role Recommendations
Suggests accurate job roles based on identified skills.

🌐 Real-Time Market Insights
With google_search, it retrieves:

- In-demand skills

- Salary ranges

- Job market requirements

📝 Resume Improvement Tips
Highlights missing elements and improvement areas.

✍️ Auto Cover Letter Generation
Creates a clean, professional cover letter in seconds.

💻 Easy to Use
Runs entirely inside Kaggle Notebook — no setup required.

🤝 Practical & Real-World Friendly
Works like a fast, AI-driven career counselor.

# 🧠 How It Works

1️⃣ Upload Resume (PDF)

The system uses pdfplumber to extract resume text.

2️⃣ Extract Skills

A custom Python script compares resume text with a pre-built skills list.

3️⃣ ADK Agent + Gemini Analysis

The agent produces:

- Key skills

- Candidate summary

- Suitable job roles

- Resume improvement suggestions

4️⃣ Google Search Tool

Fetches real-time insights:

- Trending skills in 2025

- Salary expectations

- Market demand

5️⃣ Cover Letter Generation

Gemini creates a personalized cover letter based on skills + summary.

6️⃣ Display Results

All outputs show cleanly inside the notebook.

![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/aB7_ojfFXqI3JpdkMLaE8.png).
# 🛠 Technologies Used
1.Google ADK (Agent Development Kit).

2.Gemini 2.5 Flash Lite.

3.google_search Tool.

4.Python.

5.pdfplumber (for PDF extraction).

6.Kaggle Notebook environment.

# 📂 Project Structure

```
Smart-career-application/
│
├── notebooks/
│   └── SCAA_notebook.ipynb        # Main Kaggle notebook
│
├── data/
│   └── sample_resume.pdf          # Demo PDF for testing
│
├── Images/
│   ├── SCAA.png
│   └── flowchart.png
│
├── README.md                      # Project documentation
└── requirements.txt               # Required libraries

```

# 📦 Requirements

This project requires the following Python libraries:

```
google-adk
google-genai
pdfplumber
pandas
numpy
kaggle_secrets

```
All libraries are pre-installed in Kaggle notebooks.
No local installation is required.

# ▶️ How to Run the Project

1. Upload your resume PDF to Kaggle.

2. Run the notebook cells in order.

3. The system will:

- Extract skills

- Summarize your profile

- Recommend job roles

- Retrieve market insights

- Generate a cover letter

All results appear directly in notebook output cells.

# 🎯 Key Features

✔ Resume understanding

✔ Skill extraction

✔ Job role recommendations

✔ Resume improvement tips

✔ Market insights using Google Search

✔ Auto-generated cover letter

✔ Runs fully in Kaggle Notebook

# ⭐ Architecture Overview

The Smart Career Application Assistant (SCAA) follows a modular pipeline architecture combining PDF processing, custom tools, LLM reasoning, and external search integration.

The architecture includes the following major components:

# A. Input Layer

User provides a PDF resume uploaded to Kaggle.

The system extracts raw text using pdfplumber.

# B. Preprocessing Layer

A custom Python skill extractor identifies relevant skills from the resume text using a predefined skills database.

The extracted skills are passed into the agent prompt for structured reasoning.

# C. AI Agent Layer (ADK + Gemini)

A single ADK agent powered by Gemini 2.5 Flash Lite processes:

- Resume summary

- Job recommendations

- Resume improvement suggestions

- Market insights

# D. Tool Integration Layer

- google_search tool extends the agent with real-time data access.

- Retrieves trending skills

- Fetches salary expectations

- Finds job role requirements

# E. Output Generation Layer

The agent produces:

- Key skills

- Summary of candidate

- Suggested job roles

- Resume improvement tips

- In-demand skills

- Market salary trends

- Professional cover letter

# F. Notebook Interface Layer

All components run inside a Kaggle Notebook.

Results are displayed to the user in structured, easy-to-read outputs.

# 🧬 Agent Prompt Template

```
You are a Smart Career Application Assistant.

Given resume text and extracted skills:
1. Summarize the candidate profile
2. Identify strengths and missing skills
3. Recommend suitable job roles
4. Suggest improvements for the resume
5. Retrieve market insights using google_search
6. Generate a short professional cover letter

```

# ⭐ 2. Architecture Summary

The Smart Career Application Assistant (SCAA) is an intelligent resume analysis system built using Google’s Agent Development Kit (ADK) and Gemini models. It automates the job preparation process by reading a resume, extracting skills, recommending suitable job roles, analyzing market demand, suggesting resume improvements, and generating professional cover letters.

The project integrates:

- PDF text extraction

- Custom skill-extraction tool

- LLM-powered reasoning

- Real-time search using google_search

- Comprehensive career guidance pipeline

- SCAA helps job seekers save time, get personalized insights, and make better career decisions with accurate, AI-driven recommendations.

# (Plan → Quiz → Evaluate → Predict Weakness → Revise → Adapt Next)
SCAA plans the analysis, quizzes the resume, evaluates skills, predicts weaknesses, revises recommendations, and adapts its outputs to provide accurate, personalized career guidance.

# 🧪 Sample Outputs

```
#Demo 4: Cover Letter Generator
name = "Priyanka"
target_role = "Junior Data Scientist"
skills_list = extract_skills(resume_text)

prompt = f"""
Write a short, professional cover letter for {name} applying to a {target_role} role.

Use these skills: {skills_list}

Structure:
- 1 short intro paragraph
- 1 paragraph about skills + impact
- 1 closing paragraph

Keep it under 200 words.
"""

response = await ask_agent(prompt)
print_final_answer(response)
```

![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/Cover_letter_generated.png)


```
import pdfplumber

resume_path = "/kaggle/input/resumemain/resumeidea.pdf"

def load_resume_from_pdf(path):
    try:
        with pdfplumber.open(path) as pdf:
            text = ""
            for page in pdf.pages:
                extracted = page.extract_text()
                if extracted:
                    text += extracted + "\n"
        return text
    except Exception as e:
        print("Error reading resume:", e)
        return None

resume_text = load_resume_from_pdf(resume_path)

print("=== RESUME TEXT EXTRACTED ===\n")
print(resume_text[:1500])   # show first part only
```


![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/Resume_Text_Extracted.png)



# ⭐ Flowchart Diagram
![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/flowchart.png?raw=true)

# ⚠️ Limitations
- Works best with English-language resumes

- PDF extraction quality depends on resume formatting

- google_search accuracy may vary by region

- Not a replacement for professional career counseling

# 📌 Future Improvements

- Adding multi-agent workflow

- Adding memory for user history

- Deploying a simple web UI

- Creating job–resume match scoring 

## 🏆 Status

✔ Completed for Google × Kaggle Agents Intensive Capstone
✔ Includes full system documentation
✔ Ready for demo & submission
