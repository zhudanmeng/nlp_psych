# HealthCheck

## MacHacks 2, McMaster University

## Inspiration
COVID-19 + online school + lockdowns has definitely been tough for a lot of us. Isolation and the lack of social interaction have caused mental health issues to arise during the pandemic.

Our group wanted to create a product that can be used by anyone to diagnose mental illness based on a patient’s choice of words.

## What it does
For this hackathon, our group built a NLP model to diagnose mental illnesses. It takes in a piece of text, whether that be a sentence or a paragraph, and diagnoses mental illnesses based on that information. Our model currently is able to detect 9 different mental illnesses.

## How we built it
Our model is built using a pre-trained BERT model. We fine-tuned the final dense layer to match our classes. The data used to train the model came from an open source scrape of the major mental health subreddits related to the 9 conditions that we focused on. We performed data preprocessing to increase the efficacy of our model.

## Challenges we ran into
Finding the data for this project definitely took our group some time. Since our project was focused on mental health, a lot of the datasets available required us to submit a form to access the data. We couldn’t find any set that was perfect for our problem, however, we came across a labelled dataset that consisted of reddit posts and their correct subreddit. We were able to use this for our problem.

The biggest challenge was creating the model. Originally, we used a bidirectional LSTM, however, it didn’t work too well. We then decided to use BERT and came across various issues in implementing the pre-trained model with our data. However, after reading documentation and figuring stuff out, we were able to create an accurate model!

## Accomplishments that we're proud of
Considering our team didn’t have too much knowledge about applied NLP, getting the model to work with an 80% accuracy was definitely our biggest accomplishment.

## What we learned
Learned a ton about NLP specifically about BERT and other models. We also learned how to preprocess data for NLP applications (removing stop words, punctuation, tokenization, etc).

## What's next for HealthCheck
- Deploy the model so that users can use our product
- Handle different data types (video, notes, etc)
- Providing a summary of facial expressions from video consultation
- Add more tools to help diagnose conditions
