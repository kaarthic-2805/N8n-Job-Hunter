# 🤖 AI Job Hunter Automation using n8n

An AI-powered workflow built with **n8n** that automates the entire job search process. The workflow extracts skills from a candidate's resume, searches LinkedIn for relevant job openings, analyzes each job using an AI model (Groq LLM), stores matching jobs in Google Sheets, and sends instant Telegram notifications.

This project helps job seekers save time by automatically discovering and filtering job opportunities based on their skills and experience.

---

## 🚀 Features

- 📄 Extracts text from a resume (PDF) stored in Google Drive.
- 🔍 Generates LinkedIn search queries dynamically.
- 🌐 Fetches job listings from LinkedIn automatically.
- 📑 Extracts detailed job descriptions from each job posting.
- 🤖 Uses Groq AI to evaluate job relevance based on the candidate's profile.
- 🎯 Filters jobs according to skills, experience, and matching criteria.
- 📊 Stores unique job postings in Google Sheets.
- 🔔 Sends Telegram notifications for newly found matching jobs.
- 🔄 Prevents duplicate job entries.
- ⏰ Runs automatically at scheduled intervals.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| Google Drive | Resume Storage |
| Google Sheets | Job Database |
| LinkedIn | Job Listings |
| Groq LLM | AI Job Matching |
| Telegram Bot | Notifications |
| JavaScript | Data Processing & Parsing |

---

## 📌 Workflow Overview

```text
Schedule Trigger
       │
       ▼
Download Resume (Google Drive)
       │
       ▼
Extract Text from PDF
       │
       ▼
Read Search Parameters (Google Sheets)
       │
       ▼
Generate LinkedIn Search URL
       │
       ▼
Fetch LinkedIn Job Listings
       │
       ▼
Extract Job Links
       │
       ▼
Loop Through Each Job
       │
       ▼
Fetch Job Details
       │
       ▼
Parse Job Information
       │
       ▼
AI Analysis (Groq LLM)
       │
       ▼
Filter & Score Jobs
       │
       ▼
Store in Google Sheets
       │
       ▼
Send Telegram Notification
```

---

## ⚙️ Workflow Components

### 1. Schedule Trigger
Starts the workflow automatically at a predefined schedule.

### 2. Google Drive
Downloads the latest resume in PDF format.

### 3. PDF Extraction
Extracts the resume content to identify skills and keywords.

### 4. Google Sheets
Reads predefined search parameters such as:
- Job Role
- Location
- Experience
- Skills

### 5. Search URL Generator
Creates dynamic LinkedIn search URLs.

### 6. LinkedIn Job Fetcher
Retrieves job listings matching the search criteria.

### 7. HTML Parser
Extracts job links and relevant information from LinkedIn pages.

### 8. Loop Processing
Processes each job listing individually.

### 9. Job Detail Extractor
Collects:
- Job Title
- Company
- Location
- Experience
- Skills
- Description
- Application Link

### 10. AI Agent (Groq LLM)
Analyzes every job posting against the resume and determines:
- Skill Match
- Experience Match
- Overall Suitability
- Recommendation

### 11. Google Sheets Update
Stores only unique and relevant job opportunities.

### 12. Telegram Notification
Sends instant notifications containing:
- Job Title
- Company
- Location
- Match Score
- Application Link

---

## 📂 Project Structure

```
Job-Hunter/
│
├── workflow.json
├── README.md
├── assets/
│   └── workflow.png
└── screenshots/
    └── execution.png
```

---

## 🎯 Use Cases

- Automated Job Search
- Resume-Based Job Matching
- AI Career Assistant
- Recruitment Automation
- Daily Job Alerts
- Personalized Job Recommendation

---

## 🔮 Future Enhancements

- Support for Indeed and Naukri
- Email Notifications
- ATS Score Calculation
- Resume Optimization Suggestions
- Company Rating Integration
- Multi-language Resume Support
- Dashboard for Job Analytics
- Auto Apply Feature

---

## 📈 Benefits

- Eliminates manual job searching.
- Provides AI-powered job recommendations.
- Saves significant time.
- Tracks newly posted jobs automatically.
- Delivers real-time notifications.
- Maintains a centralized database of opportunities.

---

## 👨‍💻 Author

**Kaarthic I.R.**

- GitHub: https://github.com/kaarthic-2805

---

## ⭐ If you found this project useful, consider giving it a Star!
