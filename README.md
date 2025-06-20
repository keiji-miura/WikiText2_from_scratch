# Tutorial codes for pretraining minGemma model with WikiText2

## Installation:
conda create -n minGemma python=3.11  
conda activate minGemma  
conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=11.8 -c pytorch -c nvidia  

## Special requirements:
pip install accelerate>=0.26.0  
pip install "numpy<2"

## To speed up on laptops, modify the following command:
args = TrainingArguments(fp16=True, ...(the following arguments are the same as before.))  
refefence: https://huggingface.co/docs/transformers/main/en/perf_train_gpu_one  
(You can use bf16 instead on desktops.)
