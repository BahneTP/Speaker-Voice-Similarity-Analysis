# Speaker Voice Similarity Analysis and Evaluation

This repository contains the implementation for analyzing speaker voice similarity using the **WavLM** pre-trained speech model.

## Overview

The project evaluates the WavLM model's ability to differentiate speakers based on voice similarity, using embeddings derived from audio samples. The analysis includes both quantitative metrics (e.g., accuracy, confusion matrix) and visualization techniques (e.g., t-SNE plots) to assess model performance.

## Dataset

- **Accents of the British Isles (ABI-1) Corpus**: Includes recordings from 14 British accents.
- Only `.wav` files labeled as `shortpassage` are used for analysis.
- Preprocessing steps include resampling to 16kHz and ensuring mono-channel audio.

## Pre-Trained Model

- **WavLM Base+**: A self-supervised speech model from HuggingFace, optimized for speaker verification tasks.
- Embedding extraction and similarity calculations leverage cosine similarity metrics.

## Implementation

- Written in Python, utilizing libraries like HuggingFace Transformers and PyTorch.
- Core steps:
  1. Preprocessing `.wav` files.
  2. Extracting embeddings using WavLM.
  3. Calculating similarity metrics between embeddings.
  4. Evaluating model performance using quantitative metrics and visualizations.

## Evaluation

- Metrics:
  - Accuracy
  - Precision, Recall, and F1-Score
  - Confusion Matrix
- Visualization:
  - t-SNE plots for dimensionality reduction.
  - Heatmaps showing inter-accent and intra-accent similarities.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/BahneTP/Speaker-Voice-Similarity-Analysis.git
