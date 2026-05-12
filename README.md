# Energy-Advisor-Chat
An AI-powered energy advisor built with n8n. Integrates real-time electricity prices (Elering API) and local weather data to provide context-aware energy-saving recommendations.

<img width="1695" height="893" alt="1" src="https://github.com/user-attachments/assets/332ca1c6-27c9-4c46-822c-1d82658498a6" />

<img width="1682" height="897" alt="2" src="https://github.com/user-attachments/assets/4c0b6d5b-fc65-41af-b1f9-e7eadfec40ea" />

# ⚡ Smart Energy Advisor Agent (n8n + Gemini)

A context-aware AI automation workflow designed to provide real-time energy consumption advice for households in **Kotka, Finland**. This project integrates live electricity market data with local weather conditions to generate intelligent, actionable recommendations.

## 🌟 Overview
In the current energy landscape, price volatility makes consumption timing critical. This tool acts as a **Decision Support System (DSS)**, helping users decide when to run high-energy appliances (like washing machines or heat pumps) by analyzing:
- **Real-time Spot Prices:** Fetched from the Elering API (Nord Pool market).
- **Environmental Context:** Local weather data for Kotka to suggest passive heating/cooling strategies.
- **AI Reasoning:** Using Google Gemini 2.0 Flash to synthesize data into human-readable advice.

## 🚀 Key Features
- **Data Integration:** Combines heterogeneous data sources (API & Manual/Static nodes).
- **Smart Logic:** Uses JavaScript for safe data parsing and error handling.
- **Multi-lingual Capability:** Processes data in a Finnish context while providing outputs in English for international professional standards.
- **Agentic Workflow:** Employs an AI Agent with a system-level "persona" for consistent advisory quality.

## 🛠️ Tech Stack
- **Automation:** [n8n](https://n8n.io/)
- **AI Model:** [Google Gemini 2.0 Flash](https://aistudio.google.com/)
- **Data Source:** Elering Public API (Electricity Prices)
- **Language:** JavaScript (Node.js environment)

## 📦 Installation & Setup
1. **Import Workflow:** Download the `kotka-energy-advisor-workflow.json` from this repo and import it into your n8n instance.
2. **API Credentials:** - Obtain a free API Key from [Google AI Studio](https://aistudio.google.com/).
   - Add the key to the **Google Gemini(PaLM) Api** node in n8n.
3. **Trigger:** Use the **Chat Trigger** to interact with the agent.

## 📝 Example Output
> **User:** "Should I do the laundry now?"
> **Agent:** "Current electricity price is 92.85 EUR/MWh (Moderate). Since it's 12°C and sunny in Kotka, I recommend air-drying your clothes outdoors to save energy. It's a fair time to use the machine, but avoid the tumble dryer."

---
**Author:** Zahra  
*Master of Engineering Student at Xamk (South-Eastern Finland University of Applied Sciences)*
