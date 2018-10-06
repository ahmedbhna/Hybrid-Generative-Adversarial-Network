#  Hybrid-Generative-Adversarial-Network 
This code is a representative of the code used to run experiments for the paper [Deep Generative image model using a hybird system of  Multi-Adversarial Networks]
 The paper is accepted and puplished in 2017 Intl Conf on Advanced Control Circuits Systems (ACCS) Systems & 2017 Intl Conf on New Paradigms in Electronics & Information Technology (PEIT)
 https://ieeexplore.ieee.org/document/8303052.
 The First author is Ahmed M Albhnasawy, Second author is Dr Yasser omar and Dr Essam Alfakharany.
 With the current code you can run GMAN with 1 or more discriminators and either adding conditional information to generate images based on specific condition which is the class label (N=10)
 
 
 Code used while training MNIST:
 python GMAN.py --dataset mnist --num_disc 1 --lam 0. --path mnist/arith1_0 --objective modified --num_hidden 128.
 
 
 $ python GMAN.py --dataset mnist --num_disc 1 --lam 0. --path testing_dataset
 
  to load data use the command:
  python download.py mnist
  
conditions :

The dataset should be image files or a `.npy` array with shape `(dataset_size, 32, 32, num_channels)`. Set the flag `--dataset` and give the path to the `.npy` array or the directory of images to load.

You should also set the `--path` parameter to the path where you want to save the results. It won't work otherwise.

The code automatically normalizes the data to [-1, 1].
