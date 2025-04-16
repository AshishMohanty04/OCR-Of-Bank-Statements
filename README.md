

# 🧾 Document OCR, Analysis, and Visualization Web App

This project is a **Gradio-based web application** that allows users to upload or fetch document images (like Salary Slips, Profit and Loss Statements, or Checks), extract key data using **OCR (PaddleOCR)** and **Cohere LLM**, and visualize the results using **Bar Plots** or **Pie Charts**.

---

## 🔧 Features

- 🔍 **OCR Text Extraction**: Uses PaddleOCR for high-accuracy text recognition.
- 🧠 **LLM-Powered Data Extraction**: Cohere's language model parses specific values from the text (e.g., Net Salary, Bank Name).
- 📊 **Interactive Visualizations**: Displays extracted data in bar/pie charts with Matplotlib.
- ☁️ **Cloudinary Integration**: Fetch random document images from Cloudinary storage.
- 🖼️ **Multi-image Gallery Support**: View fetched images and corresponding visualizations side-by-side.
- 💡 **Gradio UI**: Simple, clean interface for uploading files or fetching from the cloud.

---

## 📦 Tech Stack

- **Python**
- **Gradio** - UI
- **PaddleOCR** - Optical Character Recognition
- **Cohere** - Language model for key information extraction
- **Cloudinary** - Cloud image hosting
- **Matplotlib** - Data visualization
- **OpenCV** & **PIL** - Image processing

---

## 🖼️ Supported Document Types

- Salary Slip
- Profit and Loss Statement
- Check

Each document type has specific key fields to extract.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/document-ocr-visualizer.git
cd document-ocr-visualizer
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

<details>
<summary>📌 Required Libraries</summary>

- paddleocr
- cohere
- numpy
- opencv-python
- matplotlib
- pandas
- gradio
- cloudinary
- requests
- Pillow
</details>

### 3. Configure Environment Variables

Replace these placeholders in the script with your actual credentials:

```python
# Cohere
api_key = "YOUR_COHERE_API_KEY"

# Cloudinary
cloud_name = "YOUR_CLOUD_NAME"
api_key = "YOUR_CLOUDINARY_API_KEY"
api_secret = "YOUR_CLOUDINARY_SECRET"
```

> 🔐 Consider using environment variables or a `.env` file instead of hardcoding.

### 4. Launch the App

```bash
python app.py
```

Gradio UI will open in your browser.

---

## 🧪 Usage Guide

- **Upload Files Tab**:
  - Upload one or more images of Salary Slips / P&L statements / Checks.
  - Select document type and chart type.
  - Click **Process Uploaded Files**.

- **Cloudinary Images Tab**:
  - Choose document type and how many images to fetch.
  - Click **Fetch and Process Cloudinary Images**.
  - See the fetched images, extracted info, and visualizations.

---

## 📷 Sample Output

- Extracted info in table format
- Side-by-side image gallery
- Charts (bar or pie) visualizing extracted numeric data

---

## ⚠️ Disclaimer

This tool relies on OCR and LLMs, so results may vary with image quality and formatting. Always validate critical information manually.

---

## 🙌 Acknowledgments

- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)
- [Cohere](https://cohere.com/)
- [Gradio](https://gradio.app/)
- [Cloudinary](https://cloudinary.com/)

---

