# ProNoG
## Description

The repository is organised as follows:

- **data**: data folder contains data we use in all experiments.
- **GP/graphcl/DSSL/models**: this four folders contain four model architectures for respective pretraining tasks specified in the paper. 
- **downprompt**: `downprompt_metanet.py` contains the codes for our condition-net implementations.
- **preprompt**: `preprompt_new1.py` is the main code for pretraining.
  

## Package Dependencies

- python 3.8.16
- pytorch 1.10.1
- cuda 11.3
- pyG 2.1.0

## Running experiments

### Node Classification
1. Homophily datasets: run Python files whose names contain the strings 'homo' and 'NC'.
2. Heterophily datasets: run Python files whose names contain the strings 'hetero' and 'NC'.

You can change the `dataset` parameter to train and evaluate on other datasets. You can excuate the codes for both pretraining and downstream prompting, otherwise, please refer to pretraining codes under `pretrain_backup` folder.

Especially, we pretrained DSSL for ENZYMES. Please go to DSSL folder to implement the pretraining and downstream prompting (i.e. `ENZYMES_pretrain.py`, `ENZYMES_prompt_NC.py`, `ENZYMES_prompt_GC.py`).

### Graph Classification
1. Homophily datasets: run Python files whose names contain the strings 'homo' and 'GC'.
2. Heterophily datasets: run Python files whose names contain the strings 'heteo' and 'GC'.
