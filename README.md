# Sentiment Analysis with Zero-Shot Classification

This project uses a pre-trained **zero-shot classification** model from Hugging Face's Transformers library to analyze the sentiment of customer reviews. Zero-shot classification enables the model to classify text into predefined categories without needing further training, making it ideal for quick, flexible analysis of sentiment or other types of content categorization.

## Overview

This code takes a list of customer reviews and analyzes each one to determine its sentiment: **positive**, **negative**, or **neutral**. Using Hugging Face's `facebook/bart-large-mnli` model, it identifies the most likely sentiment and provides a confidence score for each classification.

## Requirements

- Python 3.7+
- Hugging Face Transformers library
- Pandas

You can install the required libraries with: pip install transformers pandas

## Usage

1. Clone the repository or copy the code into your Python environment.
2. Run the code to classify each review in the predefined `reviews` list.

### Code Highlights
- **Zero-Shot Classification Model**: The `facebook/bart-large-mnli` model from Hugging Face is used for sentiment classification.
- **Candidate Labels**: Sentiment labels ("positive," "negative," "neutral") are defined and applied across each review.
- **Confidence Scores**: Each sentiment prediction comes with a confidence score, indicating the model's certainty.

### Output
The output displays each review, a preview of its content, the predicted sentiment, and the confidence score.

## Customization

To analyze a different set of reviews, update the reviews list with your own text. You can also change the candidate_labels list to classify text by other custom categories.

## License
This project is open-source and available for modification and redistribution.
