
## N8n AI Workflow Automations 🚀

[![n8n](https://img.shields.io/badge/Automation-n8n-orange?logo=n8n)](https://n8n.io)
[![AI](https://img.shields.io/badge/AI-Google%20Gemini-blue?logo=google)](https://deepmind.google/technologies/gemini/)
[![Telegram](https://img.shields.io/badge/Chat-Telegram-2CA5E0?logo=telegram)](https://telegram.org)
[![License](https://img.shields.io/badge/License-MIT-green)](#license)

A suite of **n8n** workflows powered by **Google Gemini AI** to automate and optimize academic work, team communication, and daily task management.

---

## 📌 Table of Contents

* [Overview](#overview)
* [Workflows](#workflows)

  * [AI-Powered Academic Assignment Generator](#ai-powered-academic-assignment-generator)
  * [AI Assistant](#ai-assistant)
  * [AI Manager](#ai-manager)
* [Installation & Setup](#installation--setup)
* [Usage](#usage)
* [License](#license)

---

## Overview

This repository provides **ready-to-import** n8n workflows that combine AI-driven text generation, data formatting, and messaging automation.

Perfect for:

* 📚 **Academia:** Generate well-structured assignments from raw data.
* 📩 **Productivity:** Summarize and triage incoming emails.
* 👥 **Team Management:** Send daily task updates and motivational recaps.

---

## Workflows

### AI-Powered Academic Assignment Generator

Generates a fully formatted academic assignment document from JSON input.
**Features:**

* Dynamic HTML generation from structured data.
* AI-driven content creation using Google Gemini Chat Model.
* Strict academic formatting (12pt Times New Roman, double spacing, 1-inch margins).
* Hierarchical structure with bold titles, headings, and subheadings.
  **Prerequisites:**
* n8n credential for Google Gemini (PaLM) API.
* JSON input with: Faculty, Department, Name, Course, Level, Reg No, Date, Questions, Answers.

### AI Assistant

Smart email triage that extracts, summarizes, and forwards key points to Telegram.
**Features:**

* Email parsing from Gmail or other providers.
* Concise AI summarization + follow-up task suggestions.
* Formatted Telegram output with HTML styling and emojis.
  **Prerequisites:**
* n8n credentials for Google Gemini and Telegram APIs.
* Email trigger providing incoming message content.

### AI Manager

Daily AI-powered team assistant that prioritizes tasks and sends motivational messages.
**Features:**

* Automated daily execution via Schedule Trigger.
* Task aggregation sorted by urgency.
* Motivational morning recap with AI-generated "food for thought".
* Telegram delivery to team chat.
  **Prerequisites:**
* n8n credentials for Google Gemini and Telegram APIs.
* Access to a task data source for incomplete item queries.

---

## Installation & Setup

**Clone Repository:**

```bash
git clone https://github.com/DavidGaso1/N8n-Automation/n8n-ai-workflows.git
cd n8n-ai-workflows
```

**Import Workflows into n8n:**

1. Open your n8n instance.
2. Click *Import Workflow* and select the `.json` file from `/workflows`.

**Configure Credentials:**

* Set up Google Gemini (PaLM) API credentials.
* Add Telegram Bot API token (for AI Assistant & AI Manager).
* (Optional) Configure email credentials for Gmail/IMAP integration.

**Adjust Inputs & Triggers:**

* Update JSON structure or email triggers as per your needs.

---

## Usage

* **Academic Assignment Generator:** Provide the required JSON payload → Generates an HTML document with strict academic formatting.
* **AI Assistant:** Runs on incoming email → Sends a summary, key points, and follow-up tasks to Telegram.
* **AI Manager:** Runs daily (default: 9:00 AM) → Sends prioritized task list + motivational message to your team.

---

## License

This project is licensed under the MIT License — see the LICENSE file for details.
