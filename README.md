# Use Examples

This repo mainly contains several running scripts to use OpenDelta to finetune lora to conduct parameter-efficient training of various task.

Thanks for the [original code](https://github.com/thunlp/OpenDelta/tree/main/examples/)

**To run the code**

## Install Pytorch
```
pip install torch --extra-index-url https://download.pytorch.org/whl/cu113
```
## Install requriments

```
pip install -r requriments.txt
```
## Install the repo
```
python setup_seq2seq.py develop
```
## To test the code
```
cd examples_seq2seq
python test_seq2seq.py configs/$job_name/$dataset_test.json
```
For instance, `python test_seq2seq.py configs/lora_t5-base_1/superglue_copatest.json`

## To train the code
```
python run_seq2seq.py configs/$job_name/$dataset.json
```
For instance, `python run_seq2seq.py configs/lora_t5-base_1/superglue_copa.json`
