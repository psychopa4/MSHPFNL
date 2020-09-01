# A Progressive Fusion Generative Adversarial Network for Realistic and Consistent Video Super-Resolution
This work is based on [Yi et al.](https://github.com/psychopa4/PFNL)
This is the TensorFlow version, and PyTorch version will be available.

## Datasets
We have selected [MM522 dataset](https://github.com/psychopa4/MMCNN) for training and collected another 20 sequences for evaluation, and in consider of copyright, the datasets should only be used for study.

The datasets can be downloaded from Google Drive, [train](https://drive.google.com/open?id=1xPMYiA0JwtUe9GKiUa4m31XvDPnX7Juu) and [evaluation](https://drive.google.com/file/d/1Px0xAE2EUzXbgfDJZVR2KfG7zAk7wPZO/view?usp=sharing).

Note that the [training](https://drive.google.com/open?id=1xPMYiA0JwtUe9GKiUa4m31XvDPnX7Juu) dataset provides Ground Truth images and Bicubic downsampling LR images, while the [evaluation](https://drive.google.com/file/d/1Px0xAE2EUzXbgfDJZVR2KfG7zAk7wPZO/view?usp=sharing) dataset provides Gaussian blur and downsampling images. Thus, please refer to ./model/base_model.py for generating Gaussian blur and downsampling images from Ground Truth images.

Unzip the training dataset to ./data/train/ and evaluation dataset to ./data/val/ .

We only provide the ground truth images and the corresponding 4x downsampled LR images by [DUFVSR](https://github.com/yhjo09/VSR-DUF).

## Environment
  - Python (Tested on 3.6)
  - Tensorflow (Tested on 1.12.0)

## Contact
If you have questions or suggestions, please open an issue here or send an email to yipeng@whu.edu.cn.