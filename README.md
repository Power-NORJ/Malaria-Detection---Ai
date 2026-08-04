# 🦟 AI Malaria Detection System

## Overview
Deep learning model for malaria detection in blood smear images using MobileNetV2 with transfer learning. Fine-tuned on Ghanaian samples.

## Performance
- **Accuracy:** 97.2%
- **Sensitivity:** 97.8%
- **Specificity:** 92.3%
- **Model Size (TFLite):** 2.54 MB
- **Test Samples:** 250 Ghanaian images

## Tech Stack
- TensorFlow / Keras
- MobileNetV2
- OpenCV
- Gradio
- Hugging Face

## Links
- **Model Page:** https://huggingface.co/NORJ/AI_Malaria_Parasite_Detector
- **TFLite Model:** https://huggingface.co/NORJ/AI_Malaria_Parasite_Detector/resolve/main/malaria_model.tflite
- **Live Demo:** [Insert Gradio link]

## How to Use

### Python:
```python
from huggingface_hub import hf_hub_download
import tensorflow as tf

model_path = hf_hub_download(
    repo_id="NORJ/AI_Malaria_Parasite_Detector",
    filename="local_finetuned_model.h5"
)
model = tf.keras.models.load_model(model_path)