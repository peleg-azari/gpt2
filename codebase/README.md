# Final Project: Build GPT-2

Please refer to the project handout for detailed instructions and an overview of the codebase.

This project comprises three parts. In the first part, you will implement important components of GPT-2 and use the
model for sentiment classification.
In the second part, you will use GPT-2 on two downstream tasks: paraphrase detection and sonnet generation.
In the third part, you will implement extensions to improve your model's performance on these tasks.

In broad strokes, Part 1 of this project targets:

* modules/attention.py: Missing code blocks.
* modules/gpt2_layer.py: Missing code blocks.
* models/gpt2.py: Missing code blocks.
* classifier.py: Missing code blocks.

To test Part 1, you will run:

* `sanity_check.py`: To test your implementation of GPT models.
* `classifier.py` : To perform required SST sentiment classification using your models. CFIMDB is optional/bonus and can be enabled with `--include-cfimdb`.

In Part 2 of this project, you will use GPT2 (via cloze-style classification) detect if one sentence is a paraphrase of 
another as well as generate sonnets via autoregressive language modeling.  

To test Part 2, you will run:

* `paraphrase_detection.py`: To perform paraphrase detection. 
* `sonnet_generation.py`: To perform sonnet generation.

Important: Adjust training hyperparameters, particularly batch size, according to your GPU's specifications to optimize performance and prevent out-of-memory errors.

## Pre-testing instructions

While there are missing code blocks that you need to implement in both of these files, the main focus of this second 
part are the extensions: how you modify your GPT2 model to improve its ability to determine if one sentence is a 
paraphrase of another as well as its ability to generate sonnets. 

## Setup instructions

Follow `setup.sh` to properly setup a conda environment and install dependencies.

## Acknowledgement

This project is adapted from a prior year's CS 224N
project [Implement BERT](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1246/project/default-final-project-handout-minbert-spr2024-updated.pdf)
.

Parts of the code are from the [`transformers`](https://github.com/huggingface/transformers)
library ([Apache License 2.0](./LICENSE)).
