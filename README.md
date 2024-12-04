# VQA_project
# Visual Question Answering (VQA)

This repository contains the code, data, and methodologies for our research on **Visual Question Answering (VQA)**. The study focuses on developing a multimodal model to handle VQA tasks for educational materials, particularly machine learning lectures. By integrating advanced natural language processing and computer vision techniques, we aim to bridge the gap between visual content and contextual language comprehension.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Results](#results)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Introduction

Our work targets the creation of a robust VQA model, tailored for complex educational materials, such as slides and transcripts from machine learning courses. We utilized cutting-edge technologies like multimodal transformers and advanced data preprocessing to enhance comprehension of visually rich content.

## Dataset

The dataset was compiled from Yeshiva University’s machine learning course and consists of:

1. Images from lecture slides.
2. Transcripts derived using tools like Deepgram.
3. Curated question-answer pairs aligned with the slides and lectures.

### Dataset Structure

The dataset includes:
- **Images**: Preprocessed to 224x224 resolution.
- **Questions and Answers**: Stored in structured JSON format.
- **Categories**: General QA, Open QA, Summarization, Information Extraction, etc.

## Model Architecture

### BLIP-CLIP VQA Model

The **BLIP-CLIP** model is a groundbreaking multimodal framework that merges the best features of **BLIP** (Bootstrapped Language-Image Pretraining) and **CLIP** (Contrastive Language–Image Pretraining). This fusion enables advanced visual and textual reasoning tailored to VQA tasks.

#### Highlights:
- **Text Encoder (BLIP)**: Captures complex language representations.
- **Vision Encoder (CLIP)**: Excels in extracting high-fidelity visual features.
- **Fusion Mechanism**: Integrates textual and visual embeddings to deliver accurate responses to VQA tasks.
- **Optimized for Education**: Fine-tuned on a specialized dataset for handling lecture-based content.

### Other Models
- **LLaVA-1.5**: Combines a vision encoder and a text encoder.
- **Pix2Struct**: Excels in visually situated language processing.
- **IDEFICS**: Open-source alternative for multimodal tasks.


### Optimizer and Loss
- **Optimizer**: AdamW with weight decay.
- **Loss Function**: Cross-Entropy Loss for classification.

## Training

Training was conducted on Google Colab using an NVIDIA A100 GPU with gradient accumulation for efficient resource utilization.

### Key Metrics:
- **ROUGE**: Measures text overlap.
- **COSINE Similarity**: Assesses semantic similarity.
- **BLEU**: Evaluates machine translation performance.

## Results

The models were evaluated across multiple metrics. The **Pix2Struct-Base** model achieved the best performance in terms of ROUGE and COSINE similarity, emphasizing the importance of longer training periods.



## Contributors

- Faaraan Farid Kazi
- Shikshit Gupta
- **Onkar Kunte**
- Yeshwanth Kesani
- Venu Khare


