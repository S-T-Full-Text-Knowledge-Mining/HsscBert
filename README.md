# Pre-trained Language Model for the Humanities and Social Sciences in Chinese

## Introduction

HsscBert represents a series of Bert pretrained-models training with the full-text in the domain of  humanity and social sciences in Chinese.  

Specifically, we constructed  Hssc_BERT, Hssc_BERT_wwm, Hssc_RoBERTa and Hssc_RoBERTa_wwm pre-training language models by [transformers/run_mlm.py](https://github.com/huggingface/transformers/blob/main/examples/pytorch/language-modeling/run_mlm.py) and [transformers/mlm_wwm](https://github.com/huggingface/transformers/tree/main/examples/research_projects/mlm_wwm). 

-  Full-text contains abstract and mainbody of one paper.
-  Data examples are in the `example` folder.


## News 
- 2023-08-01：Hssc_BERT, Hssc_BERT_wwm, Hssc_RoBERTa and Hssc_RoBERTa_wwm has been put forward with a larger pretraining corpus. 


##  How to use

### Huggingface Transformers 

The `from_pretrained` method based on [Huggingface Transformers](https://github.com/huggingface/transformers) can directly obtain Hssc_BERT, Hssc_BERT_wwm, Hssc_RoBERTa and Hssc_RoBERTa_wwm models online. 

- Hssc_BERT

```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/Hssc_BERT")

model = AutoModel.from_pretrained("KM4STfulltext/Hssc_BERT")
```

- Hssc_BERT_wwm

```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/Hssc_BERT_wwm")

model = AutoModel.from_pretrained("KM4STfulltext/Hssc_BERT_wwm")
```

- Hssc_RoBERTa

```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/Hssc_RoBERTa")

model = AutoModel.from_pretrained("KM4STfulltext/Hssc_RoBERTa")
```

- Hssc_RoBERTa_wwm 

```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/Hssc_RoBERTa")

model = AutoModel.from_pretrained("KM4STfulltext/Hssc_RoBERTa")
```


### Download Models

- The version of the model we provide is `PyTorch`. 

### From Huggingface 

Download directly through Huggingface's official website. 

- [KM4STfulltext/Hssc_BERT](https://huggingface.co/KM4STfulltext/Hssc_BERT)
- [KM4STfulltext/Hssc_BERT_wwm](https://huggingface.co/KM4STfulltext/Hssc_BERT_wwm)
- [KM4STfulltext/Hssc_RoBERTa](https://huggingface.co/KM4STfulltext/Hssc_RoBERTa)
- [KM4STfulltext/Hssc_RoBERTa_wwm](https://huggingface.co/KM4STfulltext/Hssc_RoBERTa_wwm)


## Disclaimer

- **Users can use the model arbitrarily within the scope of the license, but we are not responsible for the direct or indirect losses caused by using the content of the project.** 


##  Acknowledgment

- Hssc_BERT and Hssc_BERT_wwm were trained based on [BERT-Base-Chinese]([google-research/bert: TensorFlow code and pre-trained models for BERT (github.com)](https://github.com/google-research/bert)).
- Hssc_RoBERTa and Hssc_RoBERTa_wwm were trained based on [RoBERTa-wwm-ext, Chinese]([ymcui/Chinese-BERT-wwm: Pre-Training with Whole Word Masking for Chinese BERT（中文BERT-wwm系列模型） (github.com)](https://github.com/ymcui/Chinese-BERT-wwm)).

