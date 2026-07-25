# LLaVA ID Extraction

An end-to-end AI pipeline for automated identity document understanding using Computer Vision and Vision-Language Models.

---

## Overview

This project aims to build a modular pipeline for understanding government-issued identity documents.

The complete system is designed as multiple independent modules that together perform document classification, OCR, information extraction, identity verification, and fraud detection.

---

## Current Module

### Module 1 — Document Classification

The first module is a **Multi-Head Vision Transformer (ViT-Base)** that predicts three labels simultaneously:

- 📄 Document Type
- 🪪 Document Side (Front / Back)
- 🗺️ Issuing State

The model was trained using transfer learning on a synthetic dataset of U.S. identity documents.

---

## Model Performance

| Task | Validation Accuracy |
|------|--------------------:|
| Document Type | 100% |
| Document Side | 100% |
| Issuing State | 100% |
| Combined Prediction | 100% |

---

## Model Weights

The trained model weights are hosted on Hugging Face because GitHub does not allow uploading large model files through the web interface.

**Hugging Face Repository**

> Replace the link below after publishing your model.

```text
https://huggingface.co/your-username/llava_id_extraction
```

---

## Repository Structure

```text
llava_id_extraction/

├── document_classifier/
│   ├── README.md
│   ├── module_1_document_classifier.ipynb
│   └── label_mappings.json
│
├── assets/
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Vision Transformer (ViT-Base)

---

## Roadmap

- ✅ Module 1 — Document Classification
- ⏳ Module 2 — OCR
- ⏳ Module 3 — Vision-Language Information Extraction (LLaVA)
- ⏳ Module 4 — Identity Verification
- ⏳ Module 5 — Fraud Detection
- ⏳ Module 6 — Web Application

---

## License

Apache License 2.0
