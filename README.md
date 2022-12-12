# Installation

1. `pip3 install -r requirements.txt`]
2. get data at https://projects.mtc.ethz.ch/cheese-data and move to /data/cheese.json



# Evaluation 
For Evaluation of the pre-trained models. The parameters `lower_test_limit` and `upper_test_limit` in 
`baselines/stance_detection/< MODEL >_baseline_config.json` 
(possible choices: `bert`,`gottbert`,`longformer`,`nystromformer`)
adjust the upper and lower boundaries of text length considered in the test dataset for lengthwise evaluation. 
## BERT

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/bert_baseline_config.json`


## GottBERT

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/gottbert_baseline_config.json`


## Longformer

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/longformer_baseline_config.json`

## Nystromformer

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/nystromformer_baseline_config.json`

# Training

## BERT

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/bert_baseline_training_config.json`

## GottBERT

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/gottbert_baseline_training_config.json`


## Longformer

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/longformer_baseline_training_config.json`

## Nystromformer

`python3 baselines/stance_detection/baseline.py --overwrite_output_dir --config baselines/stance_detection/nystromformer_baseline_training_config.json`

# Models

The fine-tuned models can be found here: https://huggingface.co/ogoshi2000