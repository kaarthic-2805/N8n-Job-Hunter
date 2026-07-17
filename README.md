AI Job Hunter Automation (n8n)

An intelligent n8n workflow that automates the job search process by extracting skills from a resume, searching LinkedIn for matching jobs, analyzing job descriptions using AI, filtering relevant opportunities, storing results in Google Sheets, and sending instant Telegram notifications.

The workflow eliminates the need for manual job searching by continuously monitoring new opportunities and delivering personalized recommendations based on the candidate's profile.

🚀 Features
📄 Extracts skills and keywords directly from a PDF resume stored in Google Drive.
🔍 Generates optimized LinkedIn search URLs dynamically.
🌐 Scrapes LinkedIn job listings automatically.
📑 Extracts complete job descriptions from each job posting.
🤖 Uses an AI Agent (Groq LLM) to analyze job relevance based on the resume.
🎯 Scores and filters jobs according to skill matching and suitability.
📊 Stores unique job listings in Google Sheets.
🔔 Sends Telegram notifications whenever a new matching job is found.
⏰ Runs automatically on a scheduled interval using n8n's Schedule Trigger.
🔁 Prevents duplicate notifications through data validation.
🛠️ Workflow
Schedule Trigger starts the workflow.
Downloads the resume from Google Drive.
Extracts text from the PDF.
Reads search parameters from Google Sheets.
Generates LinkedIn search URLs.
Fetches LinkedIn job listings.
Parses HTML to extract job links.
Visits each job page.
Extracts detailed job information.
Sends the data to the Groq AI Agent for analysis.
Filters and enriches job attributes.
Stores new jobs in Google Sheets.
Sends Telegram notifications for relevant opportunities.
💻 Tech Stack
Automation: n8n
AI Model: Groq LLM
Job Source: LinkedIn
Storage: Google Sheets
Resume Source: Google Drive
Notifications: Telegram Bot
Parsing: HTML Extraction & JavaScript
Scheduling: n8n Schedule Trigger
🎯 Use Cases
Automated job searching
AI-powered job recommendation
Resume-based job matching
Personalized career assistant
Recruitment workflow automation
📈 Benefits
Saves hours of manual job searching.
Delivers only relevant job opportunities.
Automatically tracks new job postings.
Provides AI-assisted job filtering.
Enables real-time notifications for faster applications.
