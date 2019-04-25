# Hybrid DNN-HMM model for isolated digit recognition
Python implementation of a hybrid DNN-HMM models for isolated digit recognition.

Forced alignments are obtained from a GMM-HMM model and used to train the DNN.
The DNN is a simple multi-layer perceptron (MLP) implemented using scikit-learn.

### How to run

```
python3 submission.py <opt-args> train test
```

* `train` is the training data
* `test` is the test data

The optional arguments are:
* `--mode`: Type of model (`mlp`, `hmm`). Default: `mlp`
* `--niter`: Number of iterations to train the HMM. Default = 10
* `--nstate`: Number of states in HMM model. Default = 5
* `--nepoch`: Maximum number of epochs for training the MLP. Default=10
* `--lr`: Learning rate for the MLP. Default=0.01
* `--debug`: Uses only top 100 utterances for train and test

### Help

This code is based on a template provided by Shinji Watanabe (Johns Hopkins University), written for a course project.

For assistance, contact `draj@cs.jhu.edu`.
 
