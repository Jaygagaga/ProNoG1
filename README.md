# MDGPT
## Description

The repository is organised as follows:

- **data/**: contains data we use.
- **model_node/**: implements pre-training and node level downstream task.
- **model_graph/**: implements pre-training and graph level downstream task. 

## Package Dependencies

- python 3.8.16
- pytorch 1.10.1
- cuda 11.3
- pyG 2.1.0

## Running experiments

### Node Classification
Default dataset is Photo. You need to change the corresponding parameters in *preprompt.py*, *downprompt.py.py* and *execute.py* to train and evaluate on other datasets.

Pretrain and Prompt tune:
`python execute.py`


### Graph Classification
Default dataset is Photo. You need to change the corresponding parameters in *preprompt.py*, *downprompt.py.py* and *execute.py* to train and evaluate on other datasets.

Pretrain and Prompt tune:
`python execute.py`

