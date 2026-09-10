# 🎯 LeadHunter AI Desk
### Autonomous B2B Cold Outreach & AI Personalization Desktop Suite for Windows

[![Engine: VisualNEO Win](https://img.shields.io/badge/Built%20with-VisualNEO%20Win-06b6d4?style=for-the-badge&logo=windows)](https://visualneowin.com)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0284c7?style=for-the-badge&logo=windows)](https://visualneowin.com)
[![Runtime](https://img.shields.io/badge/Tech-Win32%20%2B%20Edge%20WebView2-teal?style=for-the-badge)](https://visualneowin.com)
[![License](https://img.shields.io/badge/License-MIT-emerald?style=for-the-badge)](LICENSE)
[![Binary Size](https://img.shields.io/badge/Size-%3C8MB%20Standalone-blueviolet?style=for-the-badge)](https://github.com)

> 🚀 **Built 100% with [VisualNEO Win](https://visualneowin.com)** — The modern, anti-bloat Windows Rapid Application Development (RAD) IDE.
> Unlike sluggish 150MB Electron apps, **LeadHunter AI Desk** combines native Win32 execution with modern Tailwind CSS / HTML5 UI via Microsoft Edge WebView2. 
> 
> 👉 **[Download the VisualNEO Win Free Trial](https://visualneowin.com)** to inspect, edit, and build desktop apps like this in minutes.

---

## ⚡ Why LeadHunter AI Desk?

Stop paying **$49 to $99/month** for cloud cold-email SaaS subscriptions. 

LeadHunter AI Desk runs **100% locally on your Windows machine** under a **BYOK (Bring Your Own Key)** model. You connect directly to OpenRouter (DeepSeek V3/R1, Claude 3.5 Sonnet, GPT-4o) and SMTP2GO (REST API email delivery) with zero markup, zero middlemen, and total data privacy.

| Metric | LeadHunter AI Desk (VisualNEO Win) | Typical Electron Outreach Tool |
| :--- | :--- | :--- |
| **Download Size** | **~7.4 MB** (Single executable) | 160 MB – 220 MB |
| **Startup Time** | **< 0.2 seconds** (Instant) | 2.5 – 4.0 seconds |
| **RAM Footprint** | **~35 MB** | 450 MB – 700 MB |
| **Monthly Subscription**| **$0 / Free & Open Source** | $49 – $99 / month |
| **Underlying Tech** | **Native Win32 + Edge WebView2** | Chromium + Node.js runtime |

---

## ✨ Key Features

1. **🎨 Sleek Dark-Mode UI (Tailwind CSS + WebView2):**
   - Real-time outreach KPI metrics (Total Leads, AI Drafted, Sent, Delivery Rate).
   - Interactive data table with batch selection, live status badges, and preview modal.

2. **🧠 Multi-Model AI Engine (OpenRouter API):**
   - Direct integration with **DeepSeek V3 / R1**, **Claude 3.5 Sonnet**, **GPT-4o Mini**, **Gemini 2.0 Flash**, and **Llama 3.3 70B**.
   - Dynamic prompt template editor with personalization tags: `{company_name}`, `{city}`, `{website}`, `{my_name}`, `{my_service}`.
   - Generates 1,000 hyper-personalized cold emails for pennies in API credits.

3. **📨 Firewall-Free Transactional Delivery (SMTP2GO REST API):**
   - Sends emails securely over HTTPS (Port 443) via REST API — never blocked by residential or corporate SMTP port restrictions.
   - Configurable anti-spam delay intervals (e.g. 5-10 seconds between emails to maintain pristine sender domain reputation).

4. **📂 Effortless CSV Import & Export:**
   - Drag & drop CSV files directly into the window (`leads_demo.csv` included).
   - Export outreach campaign results with a single click.

5. **🔒 100% Private & Local:**
   - Your prospects and API keys are stored locally on your machine in `config.ini`. No third-party servers ever touch your business data.

---

## 🚀 Quick Start (Running the Application)

### Method 1: Pre-Compiled Windows Executable (No installation required)
1. Go to the [**Releases**](../../releases) page.
2. Download `LeadHunterAI.exe` and `leads_demo.csv`.
3. Double-click `LeadHunterAI.exe` to run immediately on Windows 10 / 11.
4. Go to **Settings**, paste your [OpenRouter API Key](https://openrouter.ai/keys) and [SMTP2GO API Key](https://app.smtp2go.com/settings/api_keys).
5. Load `leads_demo.csv`, click **"Generate with AI"**, and start your outreach!

---

## 🛠️ How It Was Built & How to Customize in VisualNEO Win

This application was created with **VisualNEO Win**, demonstrating how anyone can build high-performance Windows software by pairing a visual drag-and-drop IDE with modern web technologies:

1. **Download & Install VisualNEO Win:**  
   Get the 30-day free trial at [**visualneowin.com**](https://visualneowin.com).
2. **Open the Publication:**  
   In VisualNEO Win, click **File > Open Publication...** and select `LeadHunterAI.pub`.
3. **Inspect the Architecture:**  
   - `LeadHunterAI.pub`: Handles native Windows events, INI file storage, window controls, and bidirectional bridge messages.
   - `app.html`: Modern, responsive HTML5 + Tailwind CSS frontend displayed via Microsoft Edge WebView2.
   - Native communication:
     ```neo
     ; Send data to WebView2 frontend
     wvPostMessage "WebBrowser1" "LOAD_CONFIG|{"model":"deepseek/deepseek-chat"}"
     
     ; Receive user actions from HTML UI
     :OnWebMessageReceived
       ...
     Return
     ```
4. **Test & Compile:**  
   - Press **F9** to run in live test mode.
   - Go to **Publication > Compile/Publish...** to generate your own standalone `.exe` or Inno Setup installer.

---

## 📄 License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for more information.

---

## 🌟 Backed by the VisualNEO Ecosystem

- **Official Website:** [https://visualneowin.com](https://visualneowin.com)
- **Developer Community & Forum:** [https://visualneo.com/forum](https://visualneo.com/forum)
- **Created with:** [VisualNEO Win](https://visualneowin.com) by [SinLíos Soluciones Digitales](https://sinlios.com)

*If you found this tool useful, star ⭐ this repository and check out [VisualNEO Win](https://visualneowin.com) to build your own lightweight desktop tools!*
