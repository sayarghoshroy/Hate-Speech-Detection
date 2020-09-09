# Hate Speech Detection

### Hate Speech Detection Task and Subtasks for HASOC 2020

#### Created Dataset with Features [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sayarghoshroy/Hate-Speech-Detection/blob/master/HASOC_tweet_engine.ipynb)

#### Links

- [Task Description](https://hasocfire.github.io/hasoc/2020/index.html)
- A directory with raw datasets can be found [here](https://drive.google.com/file/d/1565-8aeKS1Rg9IafzN0gbGo6v1lS48ri/view?usp=sharing).

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

---
