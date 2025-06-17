# sentiment-dashboard

# 🌐 Sentiment Analysis Dashboard

An interactive, visually intuitive web application for performing real-time sentiment analysis using Hugging Face's powerful natural language processing (NLP) models. Built with Streamlit, this dashboard delivers immediate emotional insights from text — styled with precision and deployed with security best practices in mind.

---

## 📌 Overview

This dashboard allows users to input any sentence or paragraph and receive:
- **Real-time sentiment classification** (positive, negative, neutral)
- **Confidence scores** visualized with **color-coded horizontal bars**
- A responsive, modern UI powered by **Streamlit**

Whether you're analyzing customer feedback, headlines, or social media, this app gives quick and interpretable results backed by a state-of-the-art transformer model.

---

## ⚙️ Tech Stack

- **Frontend & UI**: Streamlit
- **NLP Engine**: Transformers (via Hugging Face pipeline)
- **Language Model**: `distilbert-base-uncased-finetuned-sst-2-english`
- **Security**: Secrets handled via `.env` (locally) and Streamlit Secrets Manager (cloud)

---

## 🔐 Secret Management

This app uses an API key from Hugging Face for inference.

### ⚠️ Never hardcode your token!  
Keep it secure using:

#### 1. Local Development
Create a file named `.env` in the root of your project:

```env
HUGGINGFACE_API_KEY=your_actual_token
