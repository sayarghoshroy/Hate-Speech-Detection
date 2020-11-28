# Leveraging Multilingual Transformers for Hate Speech Detection

### Hate Speech Detection Task and Subtasks for HASOC 2020 <br>

<p align="center">
  <img src="https://github.com/sayarghoshroy/Hate-Speech-Detection/blob/master/illustrations/hate.jpg" width="70%">
</p>

---

#### Created Dataset with Features [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sayarghoshroy/Hate-Speech-Detection/blob/master/HASOC_tweet_engine.ipynb)

#### Links

- [Task Description](https://hasocfire.github.io/hasoc/2020/index.html)
- A directory with raw datasets can be found [here](https://drive.google.com/file/d/1565-8aeKS1Rg9IafzN0gbGo6v1lS48ri/view?usp=sharing).
- [Slide Deck](https://docs.google.com/presentation/d/1jqbs2oBXBin-5g6vonM04DxvKAPP_MkPXNNBjFmk-go/edit?usp=sharing)

#### Reliable Download of all Datasets

```bash
pip install gdown
gdown https://drive.google.com/uc?id=1565-8aeKS1Rg9IafzN0gbGo6v1lS48ri
```
#### Using the Processed Data

- Refer to the `2020_processed_data` directory
- One pickle file for each language
- Each having a dictionary structure
- Keys map you to lists containing the following:
  1. 'tweet_id': The provided tweet ID
  2. 'task_1': Label for Task 1
  3. 'task_2': Label for Task 2
  4. 'hasoc_id': Provided ID for the HASOC task
  5. 'full_tweet': The complete tweet as is
  6. 'tweet_raw_text': Pure tweet text without hashtags, smileys, ...
  7. 'hashtags': Hashtags
  8. 'smiley': Smileys
  9. 'emoji': Emojis
  10. 'url': URLs
  11. 'mentions': Mentions
  12. 'numerals': Numbers
  13. 'reserved_word': Reserved Words
  14. 'emotext': A textual description of all emojis
  15. 'segmented_hash': The hashtag text segmented into words
  
 #### Models and Features
 - [Perspective API](https://www.perspectiveapi.com/#/home) features for English and German
 - [XML-RoBERTa](https://huggingface.co/transformers/model_doc/xlmroberta.html) Model trained in multi-lingual setting
 - Other Transformer based models including [BERT](https://huggingface.co/transformers/model_doc/bert.html) and [distilBERT](https://huggingface.co/transformers/model_doc/distilbert.html)

#### Description

<p align="justify"> Detecting and classifying instances of hate in social media text has been a problem of interest in Natural Language Processing in the recent years. Our work leverages state of the art Transformer language models to identify hate speech in a multilingual setting. Capturing the intent of a post or a comment on social media involves careful evaluation of the language style, semantic content and additional pointers such as hashtags and emojis. We look at the problem of identifying whether a Twitter post is hateful and offensive or not. We further discriminate the detected toxic content into one of the following three classes: (a) Hate Speech (HATE), (b) Offensive (OFFN) and (c) Profane (PRFN). With a pre-trained multilingual Transformer-based masked LM at the base, we are able to successfully identify and classify hate speech from multiple languages. On the provided testing corpora, we achieve Macro F1 scores of 90.29, 81.87 and 75.40 for English, German and Hindi respectively while performing hate speech detection and of 60.70, 53.28 and 49.74 during fine-grained classification. In our experiments, we show the efficacy of Perspective API features for hate speech classification, and the effects of exploiting a multilingual training scheme.</p>

---
