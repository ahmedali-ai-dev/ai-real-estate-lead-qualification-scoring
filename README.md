# 🏠 AI Real Estate Lead Qualification & Scoring

AI-powered real estate lead qualification and scoring automation built with **n8n**.

This workflow communicates with potential real estate customers through Telegram, collects important lead information using an AI Agent, maintains conversation memory, qualifies prospects, calculates a lead score, and saves qualified leads to Google Sheets.

---

## 🎯 Project Overview

The goal of this automation is to help real estate businesses automatically qualify incoming leads before they reach the sales team.

Instead of manually asking every customer the same questions and organizing their information, the AI Agent handles the conversation, collects the required information, evaluates the lead, and stores qualified prospects automatically.

---

## ⚙️ Key Features

- 💬 AI-powered Telegram conversations
- 🤖 Real Estate AI Agent
- 🧠 Conversation Memory
- 📋 Automatic lead information collection
- 🎯 Lead qualification
- 📊 Lead scoring
- 📑 Qualified lead storage in Google Sheets
- 🔄 Automated Telegram replies
- 🌍 Supports natural customer conversations

---

## 🧠 Lead Qualification

The AI Agent collects and evaluates important information such as:

- Customer name
- Email
- Phone number
- Property type
- Transaction type
- Property status
- Budget
- Purchase timeline
- Payment method
- Whether the customer is the decision maker
- Previous real estate purchase experience

The collected information is then used to evaluate the quality of the lead.

---

## 📊 Lead Scoring

The workflow assigns an internal lead score based on the information collected during the conversation.

Leads are classified according to their qualification level:

- 🟢 **High-quality leads**
- 🟡 **Medium-quality leads**
- 🔴 **Low-quality leads**

Qualified leads are automatically saved to Google Sheets for further sales follow-up.

---

## 🔄 Workflow

![AI Real Estate Lead Qualification & Scoring Workflow](workflow.png)

### Workflow Flow

```text
Telegram Trigger
       ↓
Real Estate AI Agent
       ↓
Telegram Reply

AI Agent
   ├── OpenRouter Chat Model
   ├── Conversation Memory
   └── Save Qualified Lead → Google Sheets
