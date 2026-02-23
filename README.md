# 🏥 Lyudmila - Empathetic Medical Assistant

[![Kaggle](https://img.shields.io/badge/Kaggle-MedGemma%20Challenge-blue)](https://www.kaggle.com/competitions/med-gemma-impact-challenge)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-green.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Lyudmila** is an AI-powered medical assistant that conducts structured preliminary interviews with patients before their doctor's appointment. It uses **MedGemma** (via LM Studio) to gather detailed information about complaints and generates a concise, structured summary for the physician.

## 🎯 The Problem

In modern outpatient care, doctors have limited time per patient (often 10-15 minutes). This is insufficient for:
- Detailed history taking
- Exploring connections between complaints
- Understanding psychological context

**Result**: Critical information is missed, diagnosis quality suffers.

## 💡 Our Solution

Lyudmila doesn't replace the doctor — it **enhances** their work by:
1. **Collecting complaints** through a natural conversation before the appointment
2. **Asking structured follow-up questions** using MedGemma
3. **Generating a concise medical summary** with key findings
4. **Providing full transcript** for reference

The doctor receives structured information and can focus on clinical reasoning and patient interaction.

## 🌟 Key Features

- **Bilingual**: Full support for English and Russian
- **Privacy-first**: Runs 100% locally via LM Studio
- **Structured output**: AI-generated summary + full transcript
- **Empathetic design**: Natural conversation flow
- **MedGemma powered**: Uses Google's open medical model

## 📋 How It Works

📋 **Phase 1: Collection (Scripted)**  
   ↓  
🤖 **Phase 2: Detailed AI Assessment (MedGemma)**  
   ↓  
📊 **Phase 3: Summary Generation**


### Phase 1: Initial Complaint Collection
- Simple scripted dialogue to gather main complaints
- No AI needed, works offline

### Phase 2: AI-Driven Detailed Assessment
- MedGemma asks structured questions for EACH complaint
- Explores: onset, frequency, triggers, relieving factors, treatment attempts
- Maintains context throughout conversation

### Phase 3: Medical Summary Generation
- AI analyzes full transcript
- Creates structured summary by complaint
- Highlights key clinical insights

## 🚀 Quick Start

### Prerequisites

1. **Install LM Studio** from [lmstudio.ai](https://lmstudio.ai)
2. **Download MedGemma** model in LM Studio
3. Start local server on `http://localhost:1234`

### Installation

```bash
# Clone repository
git clone https://github.com/YOUR_USERNAME/lyudmila-medical-assistant
cd lyudmila-medical-assistant

# Install dependencies
pip install openai

Usage
# English version
python lyudmila_en.py

# Russian version
python lyudmila_ru.py

📊 Example Output
AI-Generated Summary for Doctor
text
COMPLAINT 1: Constant Weakness
   • Onset: Gradually over several years
   • Characteristics: Persistent throughout the day
   • Triggers: Bad mood, sadness, emptiness
   • Relieving factors: None mentioned
   • Treatment attempts: Seeking medical help

COMPLAINT 2: Difficulty Starting Things
   • Onset: Gradual, from laziness to procrastination
   • Characteristics: Lack of motivation
   • Triggers: Sadness, emptiness, depression
   • Relieving factors: Video games provide temporary relief

ADDITIONAL:
   • Context: Patient reports grief from loss of loved one
   • Special notes: Depression lasting >1 year, impacts daily hygiene

Full Transcript
text
🤖 Lyudmila: Let's go through your complaints in detail. Tell me about the first one...
👤 You: I feel constantly weak...

🧠 Technical Details
Model: MedGemma (via LM Studio)

Framework: OpenAI-compatible API

Language: Python 3.8+

Dependencies: Only openai package

Architecture: Hybrid (scripted + AI-driven)

🎥 Video Demonstration
[Link to your 3-minute video]

📄 License
MIT License - feel free to use and adapt

👥 Team
Alexander Ursu - Project Lead, Developer

AI Assistant - Code optimization, documentation

🏆 Competition
This project is submitted to the MedGemma Impact Challenge on Kaggle.

Tracks: Main Competition + Agentic Workflow Prize

📬 Contact

- GitHub: [@AlexUrsu] https://github.com/AlexUrsu
- Kaggle: [@alexanderursu] https://www.kaggle.com/alexanderursu
- GMail: ursu.alexer.vas@gmail.com

