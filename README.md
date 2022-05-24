# Deep Convolutional Neural Network to classify pneumonia patients from x-ray images

This is meant as a personal learning project to gain a deeper understanding of CNNs, data preprocessing techniques for images, and various regularization techniques (dropout, L1/L2, batch norm).

Currently all preprocessing and augmentation is done via TorchVision, and I'm also experimenting with different model architectures, kernel sizes, and strides to better understand the impact they have on the performance. 

I intend to also try Optuna or Hyperopt to automate the tuning process, but also test out a more basic approach using sci-kit learn's grid search

Currently all training is done on the gpu since windows doesn't have ROCm support for my graphics card, and remoteFX has been removed so I can't do a gpu passthrough onto my linux vm.