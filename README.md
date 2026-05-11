# 🤖 Multi-Modal AI Automation Workflow with n8n

> AI-powered automation system using Text, Voice, and Image inputs with OpenAI, Memory, and Smart Routing.

---

# 🚀 Project Overview

This repository contains an advanced **Multi-Modal AI Automation Workflow** built using **n8n**.

The workflow intelligently processes:

- 📝 Text Messages
- 🎤 Voice Messages
- 🖼️ Images

The system automatically detects the input type, analyzes the content, uses AI reasoning, stores conversational memory, and generates smart contextual responses.

This workflow demonstrates how modern AI automation can combine:
- Multi-modal input processing
- AI Agents
- Voice transcription
- Image analysis
- Conversational memory
- External API communication

into a scalable and production-ready architecture.

---

# 🧠 Workflow Architecture

```text
Webhook Trigger
      ↓
Switch Node
 ├── Text Branch
 │      ↓
 │   Set Text Field
 │      ↓
 │    AI Agent
 │      ↓
 │  HTTP Request
 │
 ├── Image Branch
 │      ↓
 │  Download Image
 │      ↓
 │  Analyze Image
 │      ↓
 │  Set Image Field
 │      ↓
 │    AI Agent
 │      ↓
 │  HTTP Request
 │
 └── Voice Branch
        ↓
   Download Voice
        ↓
 Transcribe Recording
        ↓
   Set Voice Field
        ↓
      AI Agent
        ↓
   HTTP Request
