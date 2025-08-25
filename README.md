# Emotion-Detection-in-Conversations-using-LLM

# Overview

This project focuses on detecting emotions in text using a fine-tuned transformer model. I started with a pretrained DistilBERT model and trained it on the GoEmotions dataset (27 labels + neutral).

The primary goal was to build a system that allows you to type any sentence and return the most likely emotions. I also deployed the model using Gradio on Hugging Face Spaces, allowing  it to be tested online.

# Project Steps
# 1. Dataset & Model

- Dataset: GoEmotions (Google’s dataset for emotion recognition)

- Base Model: DistilBERT (distilbert-base-uncased)

- Task: Text classification (multi-label emotions)

# 2. Fine-Tuning

- Tokenized text using Hugging Face tokenizer

- Fine-tuned with PyTorch & Hugging Face Trainer API on Colab (GPU)

- Saved model and tokenizer for later use

# 3. Evaluation

- Checked metrics like accuracy and F1-score

- Tested the model with custom sentences

Example:

Input: "I am feeling happy today."
Output: joy (0.87), excitement (0.08), neutral (0.05)

# 4. Deployment

- Built a Gradio app for live predictions

# 5. Visualization

- Inside the notebook: simple bar chart of top 3 predictions

# Tools & Libraries

- Python (Colab)

- Hugging Face Transformers

- PyTorch

- Gradio

- Demo video

- Screenshots & plots
