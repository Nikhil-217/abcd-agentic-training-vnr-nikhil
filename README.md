# abcd-agentic-training-vnr-nikhil

# Gmail auto-reply workflow using n8n
This project is an automation workflow built in n8n that listens for incoming Gmail messages, generates intelligent replies using the Gemini Chat Model, and automatically sends the response back to the sender.

## Table of contents
- [Features] (#features)
- [Prerequisites] (#prerequisites)
- [Setup] (#setup)
- [How It Works] (#how it works)
- [Repository Structure] (#repository structure)

  ##features
  - Gmail trigger: Starts when a new email arrives
  - Gemini AI integration: Generates context-aware replies
  - Gmail auto-reply: Sends responses instantly
  - Fully customizable workflow in n8n
  - No manual coding required—drag-and-drop automation

  ##prerequisites
  - n8n installed (self-hosted or cloud version)
  - A Google account with Gmail API enabled
  - Gemini API key (from Google AI Studio or Vertex AI)

  ##setup
  - Import the Workflow
     - Open your n8n instance
     - Import the workflow JSON file (gmail-gemini-workflow.json)
  - Configure Credentials
     - Set up Gmail credentials in n8n (OAuth2 recommended)
     - Add your Gemini API key in the HTTP Request node
  - Activate the Workflow
     - Turn on the workflow in n8n
     - It will now trigger whenever a new Gmail message is received

  ##how it works
  - Trigger → Gmail node detects new incoming emails
  - Process → Email content is sent to Gemini via HTTP Request
  - Generate → Gemini creates a smart reply
  - Send → Gmail node sends the reply back automatically

  ##repository structure
    .
  ├── gmail-gemini-workflow.json   # Exported n8n workflow
  ├── assets/                      # Screenshots and docs
  └── README.md

