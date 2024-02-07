conda create -n Molgpt python==3.7
conda activate Molgpt
pip install torch
conda install -c rdkit rdkit
pip install tqdm
conda install matplotlib
conda install seaborn


CUDA_VISIBLE_DEVICES=0 python train.py
CUDA_VISIBLE_DEVICES=0 python generate.py
CUDA_VISIBLE_DEVICES=0 python ring_optimize.py
