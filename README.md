# Use Examples

This repo mainly contains several running scripts to use OpenDelta to finetune lora to conduct parameter-efficient training of various task.

Thanks for the [original code](https://github.com/thunlp/OpenDelta/tree/main/examples/)

**To run the code**

## Install Pytorch


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
## tutorial
Several toy tutorials:
1. The scripts for docs/basic_usage
2. Using interactive module selection
3. Work with [OpenPrompt](https://github.com/thunlp/OpenPrompt)

## examples_text-classification
Modify a huggingface text-classification examples into a delta tuning one.
Currently, GLUE datasets are supported in the scripts. Roberta-base is used for performance checking. Read README.md inside the repo for detailed usage.

## examples_seq2seq
Modify a huggingface sequence to sequence examples into a delta tuning one.
Currently, SuperGLUE and GLUE datasets are supported in the scripts. T5-base is used for performance checking. Read README.md inside the repo for detailed usage.


## examples_image-classification
A toy example of using OpenDelta for a Computer Vision Pretrained Model (ViT). Since ViT is an experimental feature in huggingface transformers, this example is subject to Change at any moment. 

