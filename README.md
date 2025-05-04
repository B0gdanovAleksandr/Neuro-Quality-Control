# Neuro-Quality-Control
Нейроконтроль качества одела продаж

README (Russian)
Нейроконтроль качества отдела продаж

Этот проект предназначен для автоматической транскрибации, анализа и оценки телефонных разговоров в отделе продаж с помощью технологий машинного обучения и ИИ.

Основные возможности:
Автоматическая транскрибация аудиофайлов формата .mp3.
Хранение транскрипций в базе данных SQLite.
Анализ разговоров при помощи OpenAI GPT-3.5 для оценки качества звонков.
Генерация кратких отчетов и рекомендаций по улучшению.
Экспорт результатов в Excel.
Использование
Установите необходимые библиотеки:

bash
pip install gradio_client sqlalchemy openai

Подготовьте папку на Google Drive для хранения аудиозаписей и вставьте путь в переменную google_drive_path.

Перед запуском убедитесь, что у вас есть API-ключ OpenAI, и он сохранен как переменная окружения OPENAI_API_KEY.

Запустите скрипт. Он автоматически обработает все .mp3 файлы в указанной папке, транскрибирует их и выполнит анализ.

Результаты сохранятся в базу данных и файл call_analysis_results.xlsx.

Важные моменты
Для работы требует доступа к Google Drive для хранения и обработки аудио.
В качестве модели для транскрипции используется Whisper Large Turbo.
Анализ отражает качество коммуникации и содержит рекомендации по улучшению.


README (English)
Neural Quality Control for Sales Department

This project automates transcription, analysis, and evaluation of sales calls using artificial intelligence and machine learning technologies.

Main features:
Automatic transcription of .mp3 audio files.
Storage of transcriptions in an SQLite database.
Call quality analysis using OpenAI GPT-3.5.
Generation of concise reports and improvement recommendations.
Export results to Excel.
Usage
Install required libraries:

bash
pip install gradio_client sqlalchemy openai

Prepare a folder on Google Drive for storing recordings and set the path in the google_drive_path variable.

Ensure you have an OpenAI API key set as environment variable OPENAI_API_KEY.

Run the script. It will automatically process all .mp3 files in the specified folder, transcribe and analyze them.

Results will be saved in the database and exported to call_analysis_results.xlsx.

Important notes
Requires access to Google Drive for storing and processing recordings.
Uses Whisper Large Turbo model for transcription.
The analysis evaluates communication quality and provides improvement tips.
