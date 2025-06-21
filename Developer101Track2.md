# 🔧 Track 2: Project-Based Learning Modules

**Duration:** 4 weeks  
**Goal:** Apply foundational skills to build working AI tools using TamarindTech’s live project patterns.

This track includes two core modules:
- **Voice Agent with ElevenLabs**
- **Automation Bot with n8n + Supabase**

Each module includes learning, building, and deploying a project.

---

## 🗣️ Module A: Voice Agent for Restaurants *(Weeks 3–4)*

### 🎯 Project Goal
Build a voice-based assistant that can:
- Answer questions about a restaurant (location, menu, opening hours)
- Handle basic booking requests
- Send an email confirmation

### 🧠 Core Concepts
- Voice AI (text-to-speech)
- Voice Assistant workflows
- Prompt engineering for voice agents
- Integrating LLM output with audio response

### 🛠️ Tech Stack
- **ElevenLabs**: Voice Synthesis API
- **OpenAI API**: Language model for answers
- **n8n**: Automation and email notification
- **Replit**: Frontend interface (optional)

### 📚 Learning Activities
- Read: *ElevenLabs API Guide*
- Watch: *How to create a Twilio + ElevenLabs voice bot*
- Read: *n8n Email Node Tutorial*

### 💻 Build Phases
1. **Voice Assistant Core**  
   - Create a prompt template: e.g., “You are a helpful restaurant assistant...”
   - Use n8n to connect:  
     `HTTP Request → OpenAI Completion → ElevenLabs Audio → Play/Send link`

2. **Restaurant FAQ Dataset**  
   - Define: Name, address, menu, business hours  
   - Store in JSON or Supabase table  
   - Add logic to respond based on question type

3. **Booking Integration**  
   - Add user input for date, time, party size  
   - Store in Supabase or send via email  
   - Trigger confirmation response with synthesized voice

### ✅ Project Deliverable
- A demo voice agent webpage or Twilio call handler
- Source code repo with README
- Loom walkthrough video

---

## 🔄 Module B: AI Automation Bot – Receipt Parser *(Weeks 5–6)*

### 🎯 Project Goal
Build a bot that:
- Accepts receipt images
- Extracts key data (date, vendor, amount)
- Logs the result in Google Sheets or Supabase
- Sends periodic email reports

### 🧠 Core Concepts
- OCR (image-to-text)
- Data parsing
- Automation logic in n8n
- Integration with Sheets or Supabase

### 🛠️ Tech Stack
- **n8n**: Workflow automation
- **OCR API**: Google Vision API or OCR.space
- **Supabase or Google Sheets**: Data store
- **Replit**: Upload frontend (optional)

### 📚 Learning Activities
- Read: *Google Vision OCR API*
- Tutorial: *Google Sheets API with n8n*
- Blog: *How to parse receipts for bookkeeping*

### 💻 Build Phases
1. **File Upload Endpoint**  
   - Create webhook in n8n to receive uploaded image  
   - Store image temporarily

2. **Extract & Parse**  
   - Use OCR API to convert image to text  
   - Use regex or OpenAI to extract fields (e.g., vendor name, total)

3. **Store & Report**  
   - Save parsed data to Supabase table or Google Sheets  
   - Weekly summary report via email

### ✅ Project Deliverable
- Live workflow link or demo frontend
- Automated pipeline from upload → storage → report
- GitHub repo with instructions

---

## 🧾 Track 2 Summary

| Module         | Project                    | Tools                         | Deliverable              |
|----------------|----------------------------|-------------------------------|---------------------------|
| Voice Agent    | Restaurant Info & Booking | ElevenLabs, OpenAI, n8n       | Voice assistant demo      |
| Automation Bot | Receipt Parser + Logger   | OCR, n8n, Supabase/Sheets     | Upload-to-report bot      |

