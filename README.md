## Hate Speech Detection Using PyTorch (BERT Tuning)

## Hate Speech Detection: Overview

* Created a tool that predicts whether a given statement is a hate speech (with test acc. of ~71%) to classify tweets.
* Dataset contains over 110K tweets from various sources.
* Data preprocessing includes deletion of unused features while labels from different sources were appropriately changed.
* Built a classifier to fine tune a BERT model usign PyTorch.
* Compared wiht a base model of just all labeled non-hateful.
* Project was carried out to learn the deeper aspects of transformers and LLMs. 

### Resources:
**Python**: 3.9.16\
**Packages**: Numpy, Pandas, Matplotlib, Regex, TQDM, Transformers (HuggingFace), Torch, Scikit-learn\
**Installing requirements**: pip install -r requirements.txt\
**Dataset**: https://www.ims.uni-stuttgart.de/forschung/ressourcen/korpora/stance-hof/

### Data Cleaning:
* Removed columns that were targeted for person specific form of hate-speeches.
* Removed few duplicates found in the data.
* Balanced data as the disparities in counts of the labels were huge (causes bias), by downsampling.
