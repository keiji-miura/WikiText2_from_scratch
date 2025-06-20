# Tutorial codes for pretraining minGemma model with WikiText2

## installation:
conda create -n minGemma python=3.11  
conda activate minGemma  
conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=11.8 -c pytorch -c nvidia  

## special requirements:
pip install accelerate>=0.26.0  
pip install "numpy<2"

## To speed up, modify the following command:
args = TrainingArguments(fp16=True, ...(same as before))
refefence: https://huggingface.co/docs/transformers/main/en/perf_train_gpu_one
