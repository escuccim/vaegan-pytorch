# VAE-GAN-pytorch
After having spent months unsuccessfully trying to combine a GAN and a VAE I discovered the paper "Autoencoding beyond pixels using a learned similarity metric" [1] which successfully did just that. 

The general skeleton for this code was taken from [2] which implemented a smaller version of the network described in the paper. My changes were:
 - Increasing the size of the input and output images
 - Using different architectures for the models
 
Specifically, I used the decoder I had previously designed for my attempts at this, and I have also experimented with using existing ConvNet architectures for the encoder and discriminator. By using an existing architecture and modifying it I am able to initialize those models with pre-trained weights which significantly speeds up training.


## References
[1] "Autoencoding beyond pixels using a learned similarity metric" https://arxiv.org/abs/1512.09300
[2] https://github.com/lucabergamini/VAEGAN-PYTORCH 



