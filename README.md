# 🔍 Resello AI Inspector

**Resello** is an AI-powered dynamic pricing and inspection system designed to revolutionize the way used electronics (Laptops & Mobiles) are valued in the re-commerce market. 

By combining **Computer Vision (CLIP)** for visual validation and **Large Language Models (Gemini)** for damage analysis and pricing justification, Resello provides a fair, transparent, and automated valuation report in seconds.

---

## 🌍 Overview 

Resello automates the appraisal process for second-hand electronics. It guides users through a structured photo session, validates images in real-time to ensure the right angles are captured, detects physical defects, and searches live market data to recommend a competitive resale price.



---

## ✨ Key Features

- 📸 **Guided Visual Inspection:** Real-time checking of photo angles (Back, Front, Sides) using OpenAI's **CLIP** model.
- 🛠️ **Automated Damage Detection:** Deep analysis of images to detect scratches, dents, and cracks using **Google Gemini (Vision)**.
- 💰 **Dynamic Pricing Engine:** Calculates value based on age-based depreciation and condition-based penalties.
- 📡 **Market Integration:** Fetches real-time market prices for new units using **SerpApi**.
- 📝 **Explainable AI (XAI):** Generates a detailed justification for the price in **English**.
- 📄 **Professional PDF Reports:** Export your inspection results into a polished PDF document.
- 🎨 **Premium UI:** A sleek, multi-step interface built with **Streamlit**.

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-orange?style=for-the-badge)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=google&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)

- **Frontend:** Streamlit
- **Computer Vision:** OpenAI CLIP (via Transformers)
- **Large Language Model:** Google Gemini 1.5 Flash
- **Market Data:** SerpApi (Google Search API)
- **PDF Generation:** fpdf2
- **Data Logic:** LangChain, NumPy, PIL

---

## 🚀 Getting Started

### 1. Prerequisites
- Python 3.9+
- API Keys: 
  - `GOOGLE_API_KEY` (Gemini)
  - `SERPAPI_KEY` (Market Research)

### 2. Installation
```bash
# Clone the repository
git clone https://github.com/zainabayman11/ReSello-v2.git
cd ReSello-v2

# Create and activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1  # Windows

# Install dependencies
pip install -r requirements.txt
```

### 3. Configuration
Create a `.env` file in the root directory:
```env
GOOGLE_API_KEY=your_gemini_key_here
SERPAPI_KEY=your_serpapi_key_here
GEMINI_SECONDARY_KEY=optional_alternative_key
```

### 4. Run the App
```bash
streamlit run app.py
```

---

## 📸 How it Works
1. **Input Product Details:** Enter the model name and usage duration.
2. **Upload Photos:** Capture 5-6 standardized views. CLIP ensures you're uploading the correct side.
3. **AI Analysis:** Gemini scans for defects and searches for the latest market price.
4. **Get Your Report:** Download a comprehensive PDF with the final price and breakdown.

---
Developed as part of the **NTI Re-Commerce Project**. 🚀
