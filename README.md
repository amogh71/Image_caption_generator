# 🖼️ Image Caption Generator

A simple and powerful image captioning project that uses the `ViT-GPT2` transformer model from Hugging Face to generate natural language descriptions of images.

---

## 🚀 Overview

This project generates captions for images using a Vision Transformer (ViT) encoder and GPT-2 decoder. It takes any input image and returns a human-readable description. Built and tested using Google Colab.

---

## ✅ Features

- Uses `nlpconnect/vit-gpt2-image-captioning` model
- Accepts multiple input images
- Automatically converts and resizes images
- Displays the image along with the predicted caption
- Runs on both CPU and GPU

---

## 🛠️ Tech Stack

- Python
- Google Colab
- PyTorch
- Hugging Face `transformers`
- Vision Transformer (ViT)
- GPT-2
- PIL (Pillow)

---

# 📦 Dependencies

```bash
pip install --upgrade torch torchvision torchaudio transformers
---

```
📄 How It Works

1. Load the pretrained ViT-GPT2 model, processor, and tokenizer.

2. Define decoding parameters: 
   max_length = 16, num_beams = 4

3. Use a helper function: predict_step(image_paths)

   - Opens image
   - Processes via ViTImageProcessor
   - Runs inference with .generate()
   - Decodes tokens to produce a caption

Example Output:

<img width="2453" height="851" alt="image" src="https://github.com/user-attachments/assets/89b879b8-c53c-4d35-8321-f36a98df5d5e" />


🔮 Future Improvements
Build a Streamlit or Gradio web app version

Fine-tune on a custom image dataset

Add multiple language support for captions

Include image upload directly in web UI

