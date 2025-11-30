# Smart-career-application
A simple and intelligent AI-powered tool that helps job seekers analyze their resume, extract skills, get job role suggestions, check market trends, and generate professional cover letters.
![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/SCAA.png?raw=true)

# Team Members
Priyanka
Monika Dhukia
Shrishti Yadav


# Google × Kaggle Agents Intensive – Capstone Project
# 🏆 Hackathon Writeup + Full System Documentation

# 🚀 Project Overview
The Smart Career Application Assistant (SCAA) uses Google’s Agent Development Kit (ADK) and Gemini LLM to understand resumes and give helpful career guidance.
This system automatically:
Reads and extracts text from a PDF resume
Finds skills using a custom Python skill extractor
Suggests job roles that match the skills
Provides resume improvement tips
Uses Google Search to check real-time job market trends
Generates a short personalized cover letter
This makes the job preparation process much faster and easier.

# Problem Statement
Job seekers often struggle to understand what their resume communicates and which job roles they are best suited for. Reviewing a resume manually, identifying key skills, checking which roles match those skills, and researching market trends can take hours. Many people also lack guidance on how to improve their resumes or write strong cover letters. The process is time-consuming, confusing, and often leads to missed opportunities.
# ⭐ SCAA Solve this:
 1. Saves Time
The system instantly analyzes a resume, extracts skills, and provides insights that would normally take hours of manual research.
 2. Accurate Skill Identification
Automatically identifies relevant technical and soft skills from the resume using a custom skill extractor.
 3. Personalized Job Role Recommendations
Suggests job roles that match the user's skills, improving clarity and helping candidates target the right positions.
 4. Real-Time Market Insights
Using the google_search tool, the agent provides up-to-date information on:
a. In-demand skills
b. Salary trends
c.Job market requirements
d.This helps users make informed career decisions.
 5. Resume Improvement Tips
The agent highlights weaknesses or missing elements and gives clear suggestions for improving resume quality.
 6. Automated Cover Letter Generation
Creates a professional cover letter based on the resume content and extracted skills, reducing effort for job applications.
 7. Easy to Use
Everything runs inside one Kaggle notebook — no extra software or setup required.
 8. Practical and Real-World Friendly
Offers guidance similar to a career counselor but faster, more scalable, and available anytime.

# 🧠 How It Works

## Upload Resume (PDF)
The system reads your resume using pdfplumber.
## Extract Skills
A custom Python function matches your skills from a predefined skills list.
## Agent Analysis (ADK + Gemini)
The SCAA agent understands the resume and provides:

## Key skills
. Summary of the candidate

. Suitable job roles

. Resume improvement tips

. Google Search Tool

. The agent gets:

. In-demand skills for 2025
. Salary ranges

. Market trends

. Cover Letter Generation

. The agent uses resume content to create a professional cover letter.

# 🛠 Technologies Used
1.Google ADK (Agent Development Kit).

2.Gemini 2.5 Flash Lite.

3.google_search Tool.

4.Python.

5.pdfplumber (for PDF extraction).

6.Kaggle Notebook environment.

# ▶️ How to Run the Project

Upload your resume PDF to the notebook environment

Run the notebook step-by-step

The agent will extract skills and analyze your resume

View:

Summary

Job suggestions

Market insights

Cover letter

# 🎯 Features

✔ Resume understanding

✔ Skill extraction

✔ Job role recommendations

✔ Resume improvement tips

✔ Market insights using Google Search

✔ Auto-generated cover letter

✔ Runs fully in Kaggle Notebook

# 📌 Future Improvements

Adding multi-agent workflow

Adding memory for user history

Deploying a simple web UI

Creating job–resume match scoring

# ⭐ Architecture Overview

The Smart Career Application Assistant (SCAA) follows a modular pipeline architecture combining PDF processing, custom tools, LLM reasoning, and external search integration.

The architecture includes the following major components:

A. Input Layer

User provides a PDF resume uploaded to Kaggle.

The system extracts raw text using pdfplumber.

B. Preprocessing Layer

A custom Python skill extractor identifies relevant skills from the resume text using a predefined skills database.

The extracted skills are passed into the agent prompt for structured reasoning.

C. AI Agent Layer (ADK)

A single ADK agent powered by Gemini 2.5 Flash Lite processes:

Resume summary

Job recommendations

Resume improvement suggestions

Market insights

D. Tool Integration Layer

google_search tool extends the agent with real-time data access.

Retrieves trending skills

Fetches salary expectations

Finds job role requirements

E. Output Generation Layer

The agent produces:

Key skills

Summary of candidate

Suggested job roles

Resume improvement tips

In-demand skills

Market salary trends

Professional cover letter

F. Notebook Interface Layer

All components run inside a Kaggle Notebook.

Results are displayed to the user in structured, easy-to-read outputs.

# ⭐ 2. Architecture Summary

The Smart Career Application Assistant (SCAA) is an intelligent resume analysis system built using Google’s Agent Development Kit (ADK) and Gemini models. It automates the job preparation process by reading a resume, extracting skills, recommending suitable job roles, analyzing market demand, suggesting resume improvements, and generating professional cover letters.

The project integrates:

PDF text extraction

Custom skill-extraction tool

LLM-powered reasoning

Real-time search using google_search

Comprehensive career guidance pipeline

SCAA helps job seekers save time, get personalized insights, and make better career decisions with accurate, AI-driven recommendations.

# (Plan → Quiz → Evaluate → Predict Weakness → Revise → Adapt Next)
SCAA plans the analysis, quizzes the resume, evaluates skills, predicts weaknesses, revises recommendations, and adapts its outputs to provide accurate, personalized career guidance.

# ⭐ Flowchart Diagram
![Alt text](https://github.com/Priyanka651/Smart-career-application-capstone-project/blob/main/Images/Architecture.png)

 

