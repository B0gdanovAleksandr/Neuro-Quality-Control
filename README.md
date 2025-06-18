# Neuro-Quality-Control  
**Neural Quality Control System for Sales Departments**

This project automates the transcription, analysis, and evaluation of sales calls using AI and machine learning. It is designed to improve the quality of customer communication and increase team efficiency.

## 🔧 Features
- 🎙️ Automatic transcription of `.mp3` audio files using Whisper Large Turbo
- 🗂️ Storage of transcriptions in SQLite database
- 🤖 Quality analysis of conversations via OpenAI GPT-3.5
- 📊 Generation of concise reports and actionable improvement recommendations
- 📤 Export of results to Excel (`call_analysis_results.xlsx`)

## 🚀 How to Use

### 1. Install Dependencies
```bash
pip install gradio_client sqlalchemy openai
2. Prepare Your Environment
Upload .mp3 audio files to a Google Drive folder

Set the path to this folder in the variable google_drive_path

Set your OpenAI API key as environment variable:

bash
Копировать
Редактировать
export OPENAI_API_KEY=your_key_here
3. Run the Script
The script will:

Scan your folder,

Transcribe audio files,

Analyze each call,

Save results in SQLite + Excel.

📌 Requirements
Access to Google Drive for file processing

Whisper Large Turbo model for fast transcription

OpenAI API access (GPT-3.5 or newer)

📈 Business Value
This tool helps:

Improve quality control feedback cycles (from days to minutes)

Detect communication issues automatically

Train sales teams faster using insights from real calls

Note: Due to NDA restrictions, only a limited version is open-sourced. A Google Colab demo is available to test using your own OpenAI key.
