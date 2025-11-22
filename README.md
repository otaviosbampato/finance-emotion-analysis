# Finance Emotion Analysis

This project implements a fine-tuning pipeline for emotion classification on financial texts using BERT. It serves as a practical study case for understanding transformer models, tokenization strategies, and the Hugging Face ecosystem.

## Project Overview

The goal is to classify financial texts into emotional categories using a pre-trained BERT model. The pipeline handles data loading, preprocessing (tokenization), and fine-tuning.

### Model Architecture
- **Base Model:** `bert-base-cased`
- **Task:** Multi-class text classification
- **Labels:** Neutral, Happy, Fear, Surprise, Sad, Disgust, Anger

### Dataset
- **source:** [vamossyd/finance_emotions](https://huggingface.co/datasets/vamossyd/finance_emotions)
- **split:** 90% Training, 10% Testing

## Requirements

- Python 3.x
- `transformers`
- `datasets`
- `evaluate`
- GPU runtime recommended for training

## Usage

> [!TIP]
> The core logic is contained in `finance_emotions_fine_tune.py`. Ensure dependencies are installed with 
> ```bash
> pip install transformers datasets evaluate
> ``` 
> before running the script.

Run:

```bash
python3 finance_emotions_fine_tune.py
```

## Authorship

[Otávio Sbampato](https://github.com/otaviosbampato)