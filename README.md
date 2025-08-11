# Automated Facebook Content Creation & Publishing Workflow

## 📌 Overview
This repository contains an **n8n automation workflow** designed to fully automate the process of researching, generating, illustrating, and posting educational social media content for **Quality Training Solutions (QTS)**.

From **topic input** in Google Sheets → **AI-powered research & content writing** → **brand-specific image generation** → **Google Drive upload** → **automatic Facebook posting**, everything runs **end-to-end without manual intervention**.

---

## 🚀 Features

- **Automated Research**  
  Fetches the latest, most relevant data using **Tavily API** based on topics from Google Sheets.

- **AI Content Writing**  
  Uses **OpenAI GPT models** to create engaging, brand-consistent posts in Vietnamese, including statistics, facts, and a conversational style.

- **Photorealistic Image Prompt Generation**  
  Generates precise prompts for **Google Imagen API**, ensuring high-quality, realistic visuals aligned with QTS brand identity.

- **Image Upload & Storage**  
  Automatically uploads images to **Google Drive** with shareable links.

- **Facebook Auto-Posting**  
  Publishes both the post text and the generated image directly to the brand’s Facebook page via **Facebook Graph API**.

- **Google Sheets Integration**  
  Reads new topics, tracks workflow status, and updates post details (image link, Facebook post ID) back into the sheet.

- **Hands-Free Workflow**  
  Entire content creation cycle runs on schedule without user interaction.

---

## ⚙️ Prerequisites

Before running the workflow, ensure you have:

- **n8n** installed (self-hosted or cloud)
- API keys for:
  - Tavily API
  - OpenAI API
  - Google Imagen API
  - Facebook Graph API
  - Google Drive & Google Sheets OAuth credentials
- A connected Facebook Page with publishing permissions
- A Google Sheet with columns:
  - `Brief topic`
  - `Note Research`
  - `Status`
  - `Drive ảnh`
  - `bài content`
