Code used to train the following 🤗 Huggingface models:
- [`cja5553/deberta-Twitter-spam-classification`](https://huggingface.co/cja5553/deberta-Twitter-spam-classification)
- [`cja5553/xlm-roberta-Twitter-spam-classification`](https://huggingface.co/cja5553/xlm-roberta-Twitter-spam-classification)

# To use

### `deberta-Twitter-spam-classification`

```{python}
from transformers import AutoTokenizer, AutoModelForSequenceClassification
tokenizer = AutoTokenizer.from_pretrained("cja5553/deberta-Twitter-spam-classification")
model = AutoModelForSequenceClassification.from_pretrained("cja5553/deberta-Twitter-spam-classification")
```

### `xlm-roberta-Twitter-spam-classification`  

```{python}
from transformers import AutoTokenizer, AutoModelForSequenceClassification
tokenizer = AutoTokenizer.from_pretrained("cja5553/xlm-roberta-Twitter-spam-classification")
model = AutoModelForSequenceClassification.from_pretrained("cja5553/xlm-roberta-Twitter-spam-classification")
```

# Spam detection of Tweets
This model classifies Tweets from X (formerly known as Twitter) into 'Spam' (1) or 'Quality' (0). 

## Training Dataset

This was fine-tuned on the [UtkMl's Twitter Spam Detection dataset](https://www.kaggle.com/c/twitter-spam/overview) with [`microsoft/deberta-v3-large`](https://huggingface.co/microsoft/deberta-v3-large) serving as the base model.

## How to use model


## Metrics

Based on a 80-10-10 train-val-test split, the following results were obtained on the test set:
- Accuracy: 0.9779
- Precision: 0.9781
- Recall: 0.9779
- F1-Score: 0.9779


## Questions?
contact me at alba@wustl.edu
