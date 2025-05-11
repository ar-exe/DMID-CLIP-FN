# DMID-CLIP-FN
This project implements a CLIP-based model for matching medical images (mammograms) with corresponding medical reports. The model is trained to understand the relationship between medical images and their textual descriptions.
## Key Features

- Custom CLIP architecture optimized for medical imaging
- Support for medical report text processing
- Image augmentation pipeline for improved training
- Contrastive learning implementation
- Inference capabilities for matching images to medical terms
- Temperature-scaled similarity scoring
The model consists of:

- Image Encoder: Modified ResNet50 with custom projection layers
- Text Encoder: Bio_ClinicalBERT with projection layers
- Embedding dimension: 1024
- Contrastive loss with temperature scaling
- Dropout layers for regularization

## Dataset Requirements

- Medical images (mammograms) in JPEG format
- Corresponding medical reports in TXT format
- File naming convention:
  - Images: `img-XXXXX-YYYYY.jpg`
  - Reports: `ImgXXX.txt`
 
## Installation

```bash
pip install torch torchvision transformers open-clip-torch albumentations nltk scikit-learn wandb
```
