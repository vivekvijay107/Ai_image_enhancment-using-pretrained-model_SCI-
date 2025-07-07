# Ai_image_enhancment-using-pretrained-model_SCI-


# 🚀 SCI Image Enhancement Web App

Welcome to the **SCI Image Enhancement** project — a cutting-edge web application that transforms your low-light or low-quality images into stunning, visually enhanced photos using the powerful **Stable Contextual Image Enhancement (SCI)** deep learning model.

This easy-to-use app leverages state-of-the-art AI to bring out details, improve brightness and contrast, and make your images look professionally enhanced — all within a sleek, user-friendly **Streamlit** interface.

---

## ✨ Key Features

- **Simple Upload & Enhance:** Just upload your image, and watch the magic happen in real time!
- **Side-by-Side Comparison:** See the original and enhanced images displayed together for instant visual feedback.
- **Download Enhanced Images:** Save your enhanced photos with a single click.
- **Lightweight & Fast:** Runs efficiently on CPU — no expensive GPU required.
- **Open Source:** Fully transparent codebase, easy to customize or extend.

---

## 🚀 Getting Started

Follow these easy steps to get your own SCI Image Enhancer up and running:

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/sci-image-enhancement.git
cd sci-image-enhancement/SCI
````

### 2. Install all necessary Python packages

```bash
pip install streamlit torch torchvision pillow numpy matplotlib pyngrok
```

### 3. Download the pretrained SCI model weights

```bash
mkdir -p weights
wget https://github.com/vis-opt-group/SCI/raw/main/weights/medium.pt -O weights/medium.pt
```

### 4. Launch the Streamlit app locally

```bash
streamlit run app.py
```

### 5. (Optional) Expose your app publicly with Ngrok (ideal for Colab users)

```python
from pyngrok import ngrok
public_url = ngrok.connect(8501)
print("Access your app here:", public_url)
```

---

## ⚙️ How It Works

* The app loads the **SCI pretrained model** — designed specifically for enhancing images with challenging lighting and quality conditions.
* When you upload an image, it converts the picture into a format the model understands.
* The model applies enhancement filters, intelligently brightening and refining image details.
* Both the original and enhanced images are displayed side-by-side so you can immediately compare the results.
* You can download the enhanced image for your own use — perfect for photographers, content creators, or anyone wanting better-looking pictures.

---

## 📁 Project Structure

```
SCI/
├── app.py                 # Streamlit web application code
├── model.py               # SCI model architecture and loading logic
├── weights/
│   └── medium.pt          # Pretrained model weights
├── README.md              # This documentation file
└── requirements.txt       # Python dependencies list (optional)
```

---

## 📚 Dataset (Optional)

If you want to **train or fine-tune** the SCI model yourself, check out the popular **LOL Dataset** used for low-light image enhancement research:

[Download LOL Dataset](https://drive.google.com/drive/folders/1oPqz-jTf56j4PlJ4mYtkoeEVdHyAMYyS)

---


## 🤝 Contact & Contributions

Created with ❤️ by [Vivek Vijay](https://github.com/vivekvijay107).
Questions, ideas, or contributions? Open an issue or pull request!

---

Thank you for checking out this project! Enjoy enhancing your images effortlessly with SCI. 🎉

```

