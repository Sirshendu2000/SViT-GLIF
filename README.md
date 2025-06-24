# SViT-GLIF

# Installation
To install all the required dependencies, run the following command in your terminal

pip install -r requirements.txt

# Training
To train and test the SViT-GLIF model on CIFAR10 dataset, run the following commands in terminal

cd cifar10

python train.py

To train and test the SViT-GLIF model on CIFAR100 dataset, run the following commands in terminal

cd cifar100

python train.py

To train and test the SViT-GLIF model on miniImageNet dataset, run the following commands in terminal

cd mini_imagenet

python train.py

# Adversarial Attacks
To implement and test the model under adversarial attacks on CIFAR10 dataset, run the following command

cd cifar10

python --experiment FGSM
