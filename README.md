# InboxPilot – AI Email Assistant for YouTubers

## Overview
InboxPilot is an automation tool designed to help YouTubers stay on top of sponsorship offers and time-sensitive emails. Built using **n8n workflow automation** and **Google Gemini API**, this agent reduces the burden of manually reviewing, classifying, and replying to emails while still keeping the creator in full control.

## Features
- **Automatic Email Classification** – Detects whether an email is a sponsorship inquiry or a high-priority message using context analysis.  
- **Smart Draft Generation** – Prepares polite, professional responses using Gemini’s language capabilities.  
- **Custom Sponsorship Rates** – Automatically includes your base sponsorship cost (e.g., $4,999).  
- **Human-in-the-loop** – Saves responses to draft instead of sending directly, so you can review before sending.  
- **Seamless Integration** – Built entirely using n8n, requiring no additional coding.  

## How It Works
1. **Email Reception:** Your Gmail (or other mail service) receives a new email.  
2. **Classification:** The n8n workflow passes the email content to Google Gemini API, which analyzes and determines if it’s a sponsorship email or high-priority email.  
3. **Response Drafting:**  
   - For **sponsorships**: Generates a reply that accepts offers at or above your base rate, or politely negotiates if below.  
   - For **high-priority messages**: Generates a quick, professional acknowledgment with clear next steps.  
4. **Draft Saving:** The generated email is automatically saved as a draft in your email account.  
5. **Manual Review:** You, the YouTuber, verify and send the email to the brand or sender.  

## Tech Stack
- **n8n** – Workflow automation platform  
- **Google Gemini API** – LLM for classification and email drafting  
- **Gmail API (or IMAP)** – For email integration  
- **Custom Business Logic** – Sponsorship base rate handling and response templates  

## Usage
1. Set up **n8n** with Gmail (or your preferred email provider).  
2. Add **Google Gemini API** credentials.  
3. Configure the workflow to trigger on new incoming emails.  
4. Adjust your **sponsorship base rate** in the workflow.  
5. Let the agent classify and draft emails — just review and send!  
