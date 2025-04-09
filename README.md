# WikiText2_from_scratch
## Tutorial codes for pretraining minGemma model with WikiText2.

### installation:
conda create -n minGemma python=3.11 ¥n
conda activate minGemma ¥n
conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=11.8 -c pytorch -c nvidia /n

### special requirements:
pip install accelerate>=0.26.0 /n
pip install "numpy<2"
