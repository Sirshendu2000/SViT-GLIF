# SViT-GLIF

# Installation
To install all the required dependencies, run the following command in your terminal

pip install -r requirements.txt

# Datasets
Follow the steps below to download and extract each dataset into its own folder structure:
## CIFAR10
mkdir -p cifar10/dataset

cd cifar10/dataset

wget https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz

tar -xvzf cifar-10-python.tar.gz


## CIFAR100

mkdir -p cifar100/dataset

cd cifar100/dataset

wget https://www.cs.toronto.edu/~kriz/cifar-100-python.tar.gz

tar -xvzf cifar-100-python.tar.gz


## MiniImageNet

mkdir -p mini_imagenet/dataset

cd mini_imagenet/dataset

wget https://cseweb.ucsd.edu/~weijian/static/datasets/mini-ImageNet/MiniImagenet.tar.gz

tar -xvzf MiniImagenet.tar.gz

  
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

python train.py --experiment FGSM
python train.py --experiment PGD
