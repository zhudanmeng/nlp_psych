# HealthCheck

## MacHacks 2, McMaster University

Won the best healthcare hack at MacHacks 2, one of Canada's largest AI hackathons.

Devpost: https://devpost.com/software/healthcheck

## Inspiration
COVID-19 + online school + lockdowns have definitely been tough for a lot of us. Isolation and the lack of social interaction have caused mental health issues to arise during the pandemic.

Our group wanted to create a product that can be used by anyone to diagnose mental illness based on a patient’s choice of words.

## What it does
For this hackathon, our group built a NLP model to diagnose mental illnesses. It takes in a piece of text, whether that be a sentence or a paragraph, and diagnoses mental illnesses based on that information. Our model currently is able to detect 9 different mental illnesses.

## How we built it
Our model is built using a pre-trained BERT model. We fine-tuned the final dense layer to match our classes. The data used to train the model came from an open source scrape of the major mental health subreddits related to the 9 conditions that we focused on. We performed data preprocessing to increase the efficacy of our model (removing stop words, punctuation, tokenization, etc). We trained the model for only 2 epochs (limited training time), and achieved an 80% accuracy!

## Technology
- Python
- Tensorflow, Keras
- Pandas

## What's next for HealthCheck
- Deploy the model so that users can use our product
- Handle different data types (video, notes, etc)
- Providing a summary of facial expressions from video consultation
- Add more tools to help diagnose conditions
