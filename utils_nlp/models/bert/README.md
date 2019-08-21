# BERT-based Classes

This folder contains utility functions and classes based on the implementation of [PyTorch-Transformers](https://github.com/huggingface/pytorch-transformers). The classes being defined here are much easier to use than the original classes in PyTorch-Transformes as the users of these cleasses do not need to deal with some coommon PyTorch framework issues and other complexitiy. For example, Tokenier in [common.py](common.py) simplies preprocessing an input dataset for a specific NLP task; all the classes defined in this submodules unburden the user from writing the loop to train with the input dataset by mutiple epoches, and the distributed training in  [sequence_classification_distributed.py](sequence_classification_distributed.py) has an implementation to use multiple GPUs on multiple nodes distibutedly for training.  
