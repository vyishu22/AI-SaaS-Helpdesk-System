# AI SaaS Helpdesk System

An AI-powered customer support automation platform that allows users to submit support tickets, interact with an AI chatbot, and enables support agents to manage tickets with AI-generated response suggestions.

---

## Project Overview

The **AI SaaS Helpdesk System** is a full-stack application designed to demonstrate how Artificial Intelligence can automate customer support workflows.

The system performs tasks such as:

- Ticket classification
- Sentiment analysis
- Priority detection
- AI-generated responses
- FAQ generation

---

## Features

### Smart Ticket Submission
Users can submit support tickets through a web form.  
The backend automatically:
- Classifies the issue (Billing, Technical, Account, Shipping, General Inquiry)
- Detects sentiment
- Assigns priority
- Generates an AI summary

### AI Chatbot
A chatbot interface that answers customer questions using AI with empathetic responses.

### Agent Dashboard
Support agents can:
- View all tickets
- See ticket details and category
- Generate AI reply suggestions
- Update ticket status

### Auto FAQ Generator
Tickets can be converted into FAQ entries using AI and displayed on the FAQ page.

---

## Tech Stack

### Backend
- Python
- Flask
- MongoDB
- OpenRouter API (GPT model)

### Frontend
- HTML
- CSS
- JavaScript

---

## Project Structure

ai-saas-helpdesk  
│  
├── backend  
│   ├── app.py  
│   ├── routes.py  
│   ├── ai_service.py  
│   └── db.py  
│  
├── frontend  
│   ├── index.html  
│   ├── submit_ticket.html  
│   ├── dashboard.html  
│   ├── faq.html  
│   ├── style.css  
│   └── script.js  
│  
├── requirements.txt  
└── README.md  

---

## Installation

### 1️⃣ Install dependencies

pip install -r requirements.txt

### 2️⃣ Create `.env` file

OPENROUTER_API_KEY=your_openrouter_api_key  
MONGO_URI=mongodb://localhost:27017/  
DB_NAME=helpdesk_db  
PORT=5000  
FLASK_DEBUG=true  

### 3️⃣ Run the application

python backend/app.py

Open the browser:

http://localhost:5000

---

## API Endpoints

| Method | Endpoint | Description |
|------|------|------|
| POST | /api/tickets | Submit support ticket |
| GET | /api/tickets | Fetch all tickets |
| POST | /api/chat | Chat with AI assistant |
| POST | /api/suggest-reply/<ticket_id> | Generate AI reply |
| POST | /api/generate-faq/<ticket_id> | Convert ticket to FAQ |
| GET | /api/faqs | Get all FAQs |

---

##  Future Improvements

- User authentication system
- Real-time chat using WebSockets
- Email notifications for ticket updates
- Analytics dashboard for ticket insights

---

