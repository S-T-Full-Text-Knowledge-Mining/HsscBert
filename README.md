# Pre-trained Language Model for the Humanities and Social Sciences in Chinese

## Introduction

HsscBert represents a series of Bert pretrained-models training with the full-text in the domain of  humanity and social sciences in Chinese.  

Specifically, we constructed Hssc_BERT_e3, Hssc_BERT_e5 pre-training language models by [transformers/run_mlm.py](https://github.com/huggingface/transformers/blob/main/examples/pytorch/language-modeling/run_mlm.py).

-  We have trained two version of HsscBert with epoch 3 and epoch 5.
-  Full-text contains abstract and mainbody of one paper.
-  Data examples are in the `example` folder.


## News 
- 2023-08-01：HsscBERT_e3, HsscBERT_e5 has been put forward with a larger pretraining corpus. 


##  How to use

### Huggingface Transformers 

The `from_pretrained` method based on [Huggingface Transformers](https://github.com/huggingface/transformers) can directly obtain Hssc_BERT, Hssc_BERT_wwm, Hssc_RoBERTa and Hssc_RoBERTa_wwm models online. 

- HsscBERT_e3

```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/HsscBERT_e3")

model = AutoModel.from_pretrained("KM4STfulltext/HsscBERT_e3")
```

- HsscBERT_e5
  
```python
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("KM4STfulltext/HsscBERT_e5")

model = AutoModel.from_pretrained("KM4STfulltext/HsscBERT_e5")
```


### Download Models

- The version of the model we provide is `PyTorch`. 

### From Huggingface 

Download directly through Huggingface's official website. 

- [KM4STfulltext/HsscBERT_e3](https://huggingface.co/KM4STfulltext/HsscBERT_e3)
- [KM4STfulltext/HsscBERT_e5](https://huggingface.co/KM4STfulltext/HsscBERT_e5)


## Disclaimer

- **Users can use the model arbitrarily within the scope of the license, but we are not responsible for the direct or indirect losses caused by using the content of the project.** 


##  Acknowledgment

- Hssc_BERTs were trained based on [BERT-Base-Chinese]([google-research/bert: TensorFlow code and pre-trained models for BERT (github.com)](https://github.com/google-research/bert)).

