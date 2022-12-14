# RobOT: Robustness-Oriented Testing for Deep Learning Systems published at ICSE 2021
See the <a href="https://arxiv.org/pdf/2102.05913.pdf" target="_blank">ICSE2021 paper</a>  for more details. 

## Prerequisite (Py3.6 & Tf2)
The code are run successfully using Python 3.6 and Tensorflow 2.2.0.

We recommend using conda to install the tensorflow-gpu environment
```shell
conda create -n tf2-gpu tensorflow-gpu==2.2.0
conda activate tf2-gpu
```

Checking installed environments
```shell
conda env list
```

to run the code in jupyter, you should add the kernel in jupyter notebook 
```
pip install ipykernel
python -m ipykernel install --name tf2-gpu
```

then start jupyter notebook for experiments
```
jupyter notebook
```

## Files
- MNIST - experiments for MNIST dataset.
- Cifar - experimnets for CIFAR-10 dataset.

metrics.py contains proposed metrics FOL. 

train_model.py is to train the DNN model.

attack.py contains FGSM and PGD attack. 

gen_adv.py is to generate adversarial inputs for test selection and robustness evaluation. You could also use toolbox like <a href="https://github.com/cleverhans-lab/cleverhans" target="_blank">cleverhans</a> for test case generation. 

select_retrain.py is to select high-quality test cases for model retraining. 

For testing method (DeepXplore, DLFuzz, ADAPT), we use the code repository <a href="https://github.com/kupl/ADAPT" target="_blank">ADAPT</a>. 

## Coming soon
More details would be included soon. 





