# AI Image Classifier – Vision Transformer Demo

**A browser-based image classification demonstration using a pretrained Vision Transformer and Gradio.**

**Project type:** Personal AI / Computer Vision Project  
**Period:** October 2025  
**Repository:** [AI-Image-Classifier-Vision-Transformer-Demo](https://github.com/p-g-udara-dilshan/AI-Image-Classifier-Vision-Transformer-Demo)  
**Availability:** Portfolio documentation; active public deployment is not claimed unless verified separately.

---

> 🧠 **Project overview**  
> This project explores **image classification inference** using an existing pretrained **Vision Transformer (ViT)** model rather than training a model from scratch. A **Gradio** web interface lets users provide an image and inspect predicted labels and associated confidence scores.

## ✨ Features

- **Image input:** upload a photo through a browser interface.
- **Pretrained ViT inference:** run image classification using a model made available through Hugging Face Transformers.
- **Prediction display:** view predicted class labels and model-reported confidence scores.
- **Interactive demonstration:** repeat predictions with different images using the Gradio UI.
- **User-facing caveat:** model predictions can be wrong, especially for unfamiliar images or situations outside the training data.

## 🛠️ Technologies

| Area | Technology |
| --- | --- |
| Programming language | Python |
| Machine learning models | Pretrained Vision Transformer (ViT) |
| Model access / inference | Hugging Face Transformers |
| Interactive web interface | Gradio |
| Classification vocabulary | ImageNet-style classes from the pretrained model |

> **Model provenance:** The architecture and trained weights come from a pretrained model. This repository demonstrates **using that model for inference**, not original ViT training, custom dataset collection, model fine-tuning, or independently verified accuracy benchmarks.

## 🖼️ Preview

![Image classification interface and sample prediction](docs/images/classification-demo.jpg)

The image shows an example prediction from the recorded demonstration. The predicted label need not match the photographed object; this is one reason the demo is presented as a learning application rather than a guaranteed recognition service.

## 🔄 How It Works

1. Choose and upload an image in the Gradio interface.
2. The image is prepared for the pretrained model's expected input format.
3. A ViT classification model processes the image.
4. The interface displays the model's predicted class labels and confidence values.

## 🚀 Running Locally

The correct launch command depends on the **actual Python entry-point file** committed to this repository.

```bash
git clone https://github.com/p-g-udara-dilshan/AI-Image-Classifier-Vision-Transformer-Demo.git
cd AI-Image-Classifier-Vision-Transformer-Demo
python -m venv .venv
```

Activate the virtual environment:

```bash
# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS / Linux
source .venv/bin/activate
```

If this repository includes `requirements.txt`, install the project's recorded dependencies:

```bash
pip install -r requirements.txt
```

Otherwise, a typical Gradio/Transformers inference environment may require Python packages such as `gradio`, `transformers`, `torch`, and `pillow`; check the source imports before installing.

Run the **actual application entry-point** specified by the source. Do not assume it is named `app.py` unless that file exists.

> The first run may need an internet connection to download pretrained model weights. A local Python interpreter, sufficient system memory, and the model's applicable license/terms may be required.

## 🎯 Learning Outcomes

- Connecting pretrained computer-vision models to an interactive Python UI.
- Understanding image classification inputs, labels, and prediction outputs.
- Learning the difference between **pretrained inference** and **model training**.
- Interpreting prediction scores critically instead of treating them as proof of correctness.

## ⚠️ Limitations

- This is an educational demo, **not** a validated high-stakes image recognition system.
- Confidence scores do not guarantee that a prediction is correct.
- Exact model checkpoints and launch commands must be confirmed against the repository source before publication.
- No public deployment URL is asserted here.

## 🔭 Possible Improvements

- Record the exact ViT checkpoint and package versions used.
- Add clear handling for invalid file types and model loading failures.
- Include examples with correct and incorrect classifications.
- Add optional reproducible evaluation on a clearly identified test dataset.

---

## 👨‍💻 Developer

**Udara Dilshan**  
GitHub: [p-g-udara-dilshan](https://github.com/p-g-udara-dilshan)  
LinkedIn: [p-g-udara-dilshan](https://www.linkedin.com/in/p-g-udara-dilshan)  
Email: [udara.profile@gmail.com](mailto:udara.profile@gmail.com)

## 📄 Content & Usage Note

This repository is shared to document the project and the developer's work. Website content, third-party images, brand identities, and client materials may belong to their respective owners. **Do not assume the project or its media are released under an open-source license** unless a license is expressly included in the repository.
