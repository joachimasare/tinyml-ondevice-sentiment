# MIT 6.5940 Final Project: On-Device Sentiment Analysis with TinyBERT

## Overview
This project explores different ways to reduce the size of a well known LLM TinyBERT so that it can reach a target size of 1MB. TinyBert is around 56MB in its out of the box form and through using different techniques we have learned in class such as pruning and quantization. In our report we discuess the results of implementing and applying fine-grained pruning, channel pruning, and k-means quantization to TinyBERT. In our attempts, the smallest we were able to make TinyBERT was 2.99MB by using K-Means quantization and fine-grained pruning.



