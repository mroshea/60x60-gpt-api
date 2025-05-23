# 60x60 GPT Health Logging API

This repository hosts the `openapi.yaml` specification for a custom GPT that logs structured daily health data — including meals, supplements, activity, and summary notes — into a Google Sheet via Make.com.

### 📦 What’s Inside
- `openapi_60x60.yaml`: OpenAPI 3.0 spec that defines a `POST /log` endpoint for sending structured health data to a Make.com webhook.
- Supports logging:
  - Meal entries with macros
  - Supplement intake
  - Physical activity and weight trends
  - Summaries for contextual recall

### 🌐 Use Case
This project enables a GPT-based health assistant to:
- Accept conversational logs (e.g., “I had coffee shake and a burger today”)
- Convert input into structured JSON
- Send data directly to your personal 60x60 health repository via Make.com

### 🔗 How It Works
1. This file is referenced by OpenAI’s GPT Builder under **Custom GPT > Configure > Actions**.
2. GPT sends structured JSON payloads to a Make.com webhook.
3. Make.com delivers the data to a Google Sheet titled `60x60_Repository_Blank`.

---

### ⚙️ Requirements
- GitHub Pages enabled for this repo
- A working Make.com webhook scenario
- A configured Custom GPT using this OpenAPI file

### ✅ Example Use Case
> “Log my meals: coffee shake for breakfast, burger and sweet potato for lunch, steak and greens for dinner.”

Your GPT will:
- Extract structure
- Send data to the webhook
- Automatically update your Google Sheet

---

### 📜 License
MIT — feel free to fork or adapt.
