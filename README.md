# 🗣️ Speech-to-Text with Wav2Vec 2.0 and Whisper

This project focuses on building and evaluating **Automatic Speech Recognition (ASR)** systems using two state-of-the-art models — **Wav2Vec 2.0** (by Facebook AI) and **Whisper** (by OpenAI).  
The goal is to compare their performance, accuracy, and adaptability across different audio conditions and languages.

---

## 🎯 Project Overview
The objective of this project is to:
- Convert raw speech audio into accurate text transcriptions.  
- Evaluate the performance of Wav2Vec 2.0 and Whisper models on the same dataset.  
- Compare transcription accuracy, robustness to noise, and inference speed.  
- Provide insights into the strengths and best-use scenarios for each model.

---

## 🧠 Models Used

### 🔹 Wav2Vec 2.0
- Developed by **Facebook AI (Meta)**.  
- A self-supervised model that learns robust speech representations directly from raw audio.  
- Fine-tuned on labeled speech datasets for ASR tasks.  
- Works best with **clean, high-quality audio** and **language-specific fine-tuning**.

**Key Features:**
- Requires minimal labeled data for training.  
- Excellent for low-resource or domain-specific adaptation.  
- Implemented via Hugging Face Transformers (`facebook/wav2vec2-base-960h`).

---

### 🔹 Whisper
- Developed by **OpenAI**.  
- A multilingual, multitask model trained on **680,000 hours** of diverse web data.  
- Supports **speech recognition**, **language identification**, and **translation**.  
- Highly robust to noise, accents, and varied recording conditions.

**Key Features:**
- Handles **multiple languages** and noisy inputs.  
- Performs **zero-shot transcription and translation**.  

```bash
pip install torch torchaudio transformers datasets jiwer openai-whisper
