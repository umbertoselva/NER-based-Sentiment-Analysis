# NER-based-Sentiment-Analysis

This Data Science project's goal is to find out what actors and film directors are more popular among the users of the "I Just Watched" movie review subreddit (July 2022).

Tech used: `Python`, `spaCy`, `Pandas`, `NumPy`, `TensorFlow`, `Huggingface Transformers`, `Flair`

The project is divided into 6 parts.

- In [**Part 01 Reddit API**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/01_Reddit_API.ipynb) I use the `Reddit API` to create a movie review dataset from the "I Just Watched" (IJW) subreddit.
- In [**Part 02 NER with spaCy**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/02_NER_with_spaCy.ipynb) I apply Named Entity Recognition to such dataset with `spaCy` in order to extract the 'PERSON' entities, I then calculate the names' frequency in the movie reviews to find out who is more frequently mentioned.
- In [**Part 03 Kaggle Dataset**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/03_Kaggle_dataset.ipynb) I use the `Kaggle API` to get a movie review dataset on which I will later (in Part 04) fine-tune a `BERT` model for Sentiment Analysis.
- In [**Part 04 Sentiment Analysis BERT**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/04_Sentiment_Analysis_BERT.ipynb), I fine-tune a `BERT` model with `TensorFlow` on the above-mentioned Kaggle movie review dataset and then use the model to predict the sentiment of the IJW subreddit reviews.
- In [**Part 05 Sentiment Analysis distillBERT with Flair**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/05_Sentiment_Analysis_distilBERT_with_Flair.ipynb) I explore an alternative method to achieve the same result, by using a pre-built `distillBERT` model with the `Flair` library.
- In [**Part 06 NER based Sentiment Analysis**](https://github.com/umbertoselva/NER-based-Sentiment-Analysis/blob/main/06_NER_based_Sentiment_Analysis.ipynb) I finally map the people's names to the sentiment of the IJW review they appear in and I am therefore able to rank each person by their average sentiment score, i.e. their popularity among the IJW review authors.

P.S. This project is inspired by various lectures and assignments in James Briggs's awesome UDEMY course "Natural Language Processing: NLP With Transformers in Python".

