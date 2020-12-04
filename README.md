## Developing Unprecedentedly Competent Transformers for TAPE

## (Tasks Assessing Protein Embeddings)

### Overview

This is a reimplementation of the paper [Evaluating Protein Transfer Learning with TAPE by Rao et al](https://arxiv.org/pdf/1906.08230.pdf). The GitHub for the paper with the model architectures implemented in PyTorch and data is [here](https://github.com/songlab-cal/tape). Due to time and resource constraints, we focused on reimplementing the downstream tasks, passing in the unsupervised pretrained model (trained on the very large Pfam protein family dataset) weights to these downstream models. We reimplemented multiple downstream models each trained for five biological tasks: Secondary Structure (SS) Prediction, ...... (TODO: add rest of the tasks after completing). The models we reimplemented were a Transformer model, ..... (TODO: add rest of models after completing).

### Dependencies

- wget (for MacOS: run `brew install wget`)
- tensorflow 2.3.0
- numpy 1.17.3+

### Data

To download the dataset, run `download_data.sh`. This should create a /data folder in the root directory that contains two folders for the different types of data: TFRecord and raw JSON. This dataset is for the Secondary Structure task only.

### Public Implementations

- https://github.com/songlab-cal/tape
- (Deprecated TensorFlow) https://github.com/songlab-cal/tape-neurips2019
