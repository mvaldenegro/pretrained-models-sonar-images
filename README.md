# Pre-Trained Models for Sonar Images

This repository contains the public release of pre-trained models for sonar images, from our Global Oceans 2021 paper.

# Pre-Trained Models

- [ResNet20](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/resnet20v1.0)
- [MobileNets](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/mobilenetv1.0)
- [DenseNet121](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/densenetv1.0)
- [SqueezeNet](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/squeezenetv1.0)
- [MiniXception](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/minixceptionv1.0)
- [Convolutional Autoencoder (only the encoder)](https://github.com/mvaldenegro/pretrained-models-sonar-images/releases/tag/encoderv1.0)

All models except the autoencoder are available at selected input image sizes between 32x32 to 96x96.

# Usage

These models were trained using Keras 2.3.1, they can be loaded as:

    from keras.models import load_model
    model = load_model('model.hdf5')

The input shape of each model is `(s, s, 1)`, where 's' can be 32, 48, 64, 80, or 96. For example, the biggest models have input shape `(96, 96, 1)`.

# Citation

If you find these models useful, you can cite our paper:

    @inproceedings{valdenegro2021pretrained,
      title={Pre-trained Models for Sonar Images},
      author={Valdenegro-Toro, Matias and Preciado-Grijalva, Alan and Wehbe, Bilal},
      booktitle={Global OCEANS 2021},
      year={2021},
      organization={IEEE}
    }

A preprint version in arXiv will appear soon.
