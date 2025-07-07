# Ai_image_enhancment-using-pretrained-model_SCI-

# SCI Image Enhancement Web App


Enhance low-light or low-quality images using the pretrained **SCI (Stable Contextual Image Enhancement)** deep learning model with a simple Streamlit web app.

---

## Features
- Upload images (JPEG, PNG) for enhancement
- Real-time image processing with SCI model
- View original and enhanced images side-by-side
- Download enhanced images
- Runs on CPU (no GPU required)

---

## Setup & Usage

1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/sci-image-enhancement.git
   cd sci-image-enhancement/SCI
````

2. **Install dependencies:**

   ```bash
   pip install streamlit torch torchvision pillow numpy matplotlib pyngrok
   ```

3. **Download pretrained weights:**

   ```bash
   mkdir -p weights
   wget https://github.com/vis-opt-group/SCI/raw/main/weights/medium.pt -O weights/medium.pt
   ```

4. **Run the Streamlit app locally:**

   ```bash
   streamlit run app.py
   ```

5. **  Expose app publicly with ngrok (useful for Colab):**

   ```python
   from pyngrok import ngrok
   public_url = ngrok.connect(8501)
   print("Open your app here:", public_url)
   ```

---

## How It Works

* Loads the pretrained SCI model on CPU
* User uploads an image via the Streamlit interface
* Converts the image to tensor, enhances it using SCI
* Shows original and enhanced images side-by-side
* Lets user download the enhanced image

---

## Project Structure

```
SCI/
├── app.py                 # Streamlit app
├── model.py               # SCI model implementation
├── weights/
│   └── medium.pt          # Pretrained weights
├── README.md              # This file
└── requirements.txt       # (optional) dependencies list
```

---

