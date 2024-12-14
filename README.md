# MIT 6.5940 Final Project: On-Device Sentiment Analysis with TinyBERT

## Overview
This project explores different ways to reduce the size of a well known LLM TinyBERT so that it can reach a target size of 1MB. TinyBert is around 56MB in its out of the box form and through using different techniques we have learned in class such as pruning and quantization. In our report we discuess the results of implementing and applying fine-grained pruning, channel pruning, and k-means quantization to TinyBERT. In our attempts, the smallest we were able to make TinyBERT was 2.99MB by using K-Means quantization and fine-grained pruning.
### Files and How to Run:
`Task_Distilled_Model_Production.ipynb`: Running this notebook allows you to distill Bert Uncased into TinyBert that is distilled on the sentiment analysis task.

`TinyBert_to_TinierBert.ipynb`: This notebook allows you to evaluate the loaded model, finetune it, fine-grain prune the model, conduct a sesnsitivity scan to determine optimal sparsity per layer, run k-means quantization on our model, and test how well doing both fine-grained pruning and k-means quantization work. 

`Distilled_TinyBert_to_TinierBert.ipynb`: This notebook does the same as `TinyBert_to_TinierBert.ipynb`, we have it here for the purposes of showing our results from pruning and quantizing our distilled model. The model that is outputtrf by 
`Task_Distilled_Model_Production.ipynb` is used in this notebook.

`Channel_Pruning.ipynb`: This notebook allows our results for structured pruning to be reproduced.


